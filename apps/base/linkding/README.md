## Setting up a linkding user
First of all get all the pods running
`kubectl get pods -A`

Look for the linkding pod, and copy the name and run:
`kubectl exec -it <linkding-pod-name> -n <namespace> -- /bin/sh`

Then you can setup a user by running
`python manage.py createsuperuser`