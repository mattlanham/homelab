
I restructured the k8s guide on the hoarder Github:
https://github.com/hoarder-app/hoarder/tree/main/kubernetes

Given this will be comitted to git, I changed how the secrets were being handled, there is probably a 
better way of doing that, but I changed the kustomization.yaml to something that I thought would work.

Use `openssl rand -base64 36` to generate the random strings

```
kubectl -n hoarder create secret generic hoarder-secrets \
  --from-literal="NEXTAUTH_SECRET=<secret>" \
  --from-literal="MEILI_MASTER_KEY=<secret>" \
  --from-literal="NEXT_PUBLIC_SECRET=<secret>" \
  --from-literal="OPENAI_API_KEY=<secret>"
```