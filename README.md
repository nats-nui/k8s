## NUI on K8S (Experimental)

This repo manage the K8s deploy of NUI and publishes the related helm chart.
Current version of NUI on K8s deploys:
- a statefulset with NUI application
- related service
- optional ingress
- optional secret to add .creds files into the pod and use the nats credential auth

## Getting started
```
helm repo add nats-nui https://nats-nui.github.io/k8s/helm/charts
helm install nats-nui nats-nui/nui
```

## Customization
Check `values.yaml` to customize enable ingress and customize the install
