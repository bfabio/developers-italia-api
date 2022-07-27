# developers-italia-api

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v0.1.1-pre](https://img.shields.io/badge/AppVersion-v0.1.1--pre-informational?style=flat-square)

The API of Developers Italia

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ghcr.io/italia/developers-italia-api"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.className | string | `""` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0].host | string | `"chart-example.local"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"ImplementationSpecific"` |  |
| ingress.tls | list | `[]` |  |
| maxRequests | int | `nil` | Max number of requests. |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| pasetoKey | string | `""` | Base64 encoded Paseto Key. |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| postgres | object | `{"database":"developers_italia_api","host":"","password":"","port":5432,"user":""}` | External PostgreSQL connection parameters. |
| postgres.database | string | `"developers_italia_api"` | Name of PostgreSQL databse. |
| postgres.host | string | `""` | Host. |
| postgres.password | string | `""` | Password. |
| postgres.port | int | `5432` | Port. |
| postgres.user | string | `""` | User name. |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| service.port | int | `80` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |
| useExistingSecret | string | `nil` | Name of existing Kubernetes secret containing keys 'databaseDSN' and 'pasetoKey'. If not provided, a secret will be generated using values from 'pasetoKey' and 'postgres'. |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs vv1.10.0](https://github.com/norwoodj/helm-docs/releases/vv1.10.0)