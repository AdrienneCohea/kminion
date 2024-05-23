# Helm Chart

⚠️ This chart has been moved to https://github.com/redpanda-data/helm-charts/tree/main/charts/kminion . Please install this chart instead. The existing archives are still being hosted here, to not break existing deployments.

---

This chart is intentionally very light on input validation. The goal was to offer a flexible Helm chart that allows
users to deploy KMinion the way they want to. Therefore it's very flexible at the cost of less input validation, so that
you might run into runtime errors for a misconfiguration.

All available input is documented inside of the [values.yaml](./kminion/values.yaml) file.

## Installing the Helm chart

```shell
helm repo add kminion https://raw.githubusercontent.com/cloudhut/kminion/master/charts/archives
helm repo update
helm install -f values.yaml kminion kminion/kminion
```
