# ./kubernetes-manifests

:warning: Kubernetes manifests provided in this directory are not directly
deployable to a cluster. They are meant to be used with `skaffold` command to
insert the correct `image:` tags.

Use the manifests in [/release](/release) directory which are configured with
pre-built public images.

#  Port-forward the internal frontend service (ClusterIP):

kubectl port-forward service/frontend 8080:80 -n micro-services-demo

Then access it locally at:
👉 http://localhost:8080

