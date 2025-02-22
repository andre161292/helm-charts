# babybuddy

![Version: 2.3.0](https://img.shields.io/badge/Version-2.3.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v1.9.0](https://img.shields.io/badge/AppVersion-v1.9.0-informational?style=flat-square)

Helps caregivers track sleep, feedings, diaper changes, tummy time and more to learn about and predict baby's needs without (as much) guess work.

## Dependencies

| Repository | Name | Version |
|------------|------|---------|
| https://andre161292.github.io/nicholaswilde-helm-charts/ | common | ~0.1.13 |
| https://andre161292.github.io/nicholaswilde-helm-charts/ | postgres | ~0.1.0 |

## TL;DR
```console
$ helm repo add nicholaswilde https://andre161292.github.io/nicholaswilde-helm-charts/
$ helm repo update
$ helm install babybuddy nicholaswilde/babybuddy
```

## Installing the Chart
To install the chart with the release name `babybuddy`:
```console
helm install babybuddy nicholaswilde/babybuddy
```

## Uninstalling the Chart
To uninstall the `babybuddy` deployment:
```console
helm uninstall babybuddy
```
The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration

Read through the [values.yaml](./values.yaml) file. It has several commented out suggested values.
Other values may be used from the [values.yaml](../common/values.yaml) from the [common library](../common).

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`. For example,
```console
helm install babybuddy \
  --set env.TZ="America/New York" \
    nicholaswilde/babybuddy
```

Alternatively, a YAML file that specifies the values for the above parameters can be provided while installing the chart.
For example,
```console
helm install babybuddy nicholaswilde/babybuddy -f values.yaml
```

|   user   | uid |
|:--------:|:---:|
| abc |  911 |

## Troubleshooting
See [Wiki](https://github.com/nicholaswilde/helm-charts/wiki/Troubleshooting).

## Author
This project was started in 2021 by [Nicholas Wilde](https://github.com/nicholaswilde).

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)
