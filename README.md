
### Install helm chart dependency
```
helm dependency build
```

### Validate helm chart

```
helm lint
```

### Install/Upgrade helm chart

Install elasticsearch, logstash, metricbeat

```
helm upgrade --install elk . --create-namespace -n elk --set "global.kibana.enabled=false"
```

Install kibana

```
helm upgrade --install elk . --create-namespace -n elk --set "global.kibana.enabled=true"
```


### For the reference of the values to change parametes of charts follow:

[elasticsearch](https://artifacthub.io/packages/helm/elastic/elasticsearch/8.5.1)

[kibana](https://artifacthub.io/packages/helm/elastic/kibana/8.5.1)

[logstash](https://artifacthub.io/packages/helm/elastic/logstash/8.5.1)

[metricbeat](https://artifacthub.io/packages/helm/elastic/metricbeat/8.5.1)