# Setup secrets (if not already completed)

Install SOPS, and age
```
brew install sops age
```

Generate an age key:
```
age-keygen -o age.agekey
```

Create and encrypt the secrets
```
kubectl -n cloudflare-operator-system create secret generic cloudflare-secrets \
    --from-literal CLOUDFLARE_API_TOKEN=<YourApiToken> \
    --from-literal CLOUDFLARE_API_KEY=<YourAPiKey> \
    --dry-run=client -o yaml > cf-secret.yaml
```

Create an `.sops.yaml` file in `clusers/default`:
```
creation_rules:
  - path_regex: .*\.(yaml|yml)$
    encrypted_regex: "^(data|stringData)$"
    age: <yourAgePublicKey>
```

Whilst in the `clusers/default` directory, run the following to encrypt the file:
```
sops --encrypt --in-place ../../infrastructure/default/cloudflare-operator/cf-secret.yaml
```

Add the private key to the cluser (this only needs to be done once)
```
cat age.agekey |
kubectl create secret generic sops-age \
--namespace=flux-system \
--from-file=age.agekey=/dev/stdin
```

Check that it is showing up:

```
kubectl get secrets -n cloudflare-operator-system  
```