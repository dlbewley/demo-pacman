# Pac-Man Demo App

Deploy [pacman](https://github.com/dlbewley/pacman) application directly to [OpenShift](overlays/openshift) or [XKS](overlays/xks).

```bash
oc apply -k https://github.com/dlbewley/demo-pacman/overlays/openshift\?refs=demo
```

Or deploy using RHACM subscription and label ManagedClusters with `licensed/pacman=true` to match the [PlacementRule](subscription/placementrule.yaml)

```bash
oc apply -k https://github.com/dlbewley/demo-pacman/subscription\?refs=demo
```

