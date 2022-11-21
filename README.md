
### Install helm chart dependency
```
helm dependency build
```

### Validate helm chart

```
helm lint
```

### Install/Upgrade helm chart

```
helm upgrade --install elk . --create-namespace -n elk
```