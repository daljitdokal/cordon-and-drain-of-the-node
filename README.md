# Cordon and drain of the node

## Cordon and drain of the node
```bash
oc login <server url>

oc adm cordon <server node name>

oc adm drain <server node name> --grace-period=-1 --delete-local-data=true --force=true --ignore-daemonsets
```

## Uncordoned the node with:
```bash
oc adm uncordon <server node name>
```

Confirmed the node now showng as ready:
```bash
oc get nodes -o wide
```
