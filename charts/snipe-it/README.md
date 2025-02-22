# snipe-it

![Version: 1.0.5](https://img.shields.io/badge/Version-1.0.5-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v5.1.8](https://img.shields.io/badge/AppVersion-v5.1.8-informational?style=flat-square)

Open source asset management

## Dependencies

| Repository | Name | Version |
|------------|------|---------|
| https://andre161292.github.io/nicholaswilde-helm-charts/ | common | ~0.1.13 |
| https://andre161292.github.io/nicholaswilde-helm-charts/ | mariadb | ~1.0.3 |

## TL;DR
```console
$ helm repo add nicholaswilde https://andre161292.github.io/nicholaswilde-helm-charts/
$ helm repo update
$ helm install snipe-it nicholaswilde/snipe-it
```

## Installing the Chart
To install the chart with the release name `snipe-it`:
```console
helm install snipe-it nicholaswilde/snipe-it
```

## Uninstalling the Chart
To uninstall the `snipe-it` deployment:
```console
helm uninstall snipe-it
```
The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration

Read through the [values.yaml](./values.yaml) file. It has several commented out suggested values.
Other values may be used from the [values.yaml](../common/values.yaml) from the [common library](../common).

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`. For example,
```console
helm install snipe-it \
  --set env.TZ="America/New York" \
    nicholaswilde/snipe-it
```

Alternatively, a YAML file that specifies the values for the above parameters can be provided while installing the chart.
For example,
```console
helm install snipe-it nicholaswilde/snipe-it -f values.yaml
```

## Troubleshooting
See [Wiki](https://github.com/nicholaswilde/helm-charts/wiki/Troubleshooting).

## Author
This project was started in 2020 by [Nicholas Wilde](https://github.com/nicholaswilde).

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)
