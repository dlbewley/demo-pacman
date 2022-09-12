# Pac-Man Demo App

Manage the deployment of [pacman](https://github.com/dlbewley/pacman) demo application.

## Deploy App Directly

Deploy directly to [OpenShift](overlays/openshift) or [XKS](overlays/xks):

```bash
oc apply -k https://github.com/dlbewley/demo-pacman/overlays/openshift\?ref=demo
```

## Deploy App via Subscription

Or deploy using RHACM subscription:

```bash
oc apply -k https://github.com/dlbewley/demo-pacman/subscription\?ref=demo
```

Then label ManagedClusters with `licensed/pacman=true` to satisfy the [PlacementRule](subscription/placementrule.yaml).

