# gitops

![Version: 0.3.0](https://img.shields.io/badge/Version-0.3.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.0.1](https://img.shields.io/badge/AppVersion-0.0.1-informational?style=flat-square)

Harness GitOps

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://harness.github.io/helm-common | harness-common | 1.x.x |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| accessControlService.basePath | string | `"api/"` |  |
| accessControlService.defaultSchemes | string | `"http"` |  |
| accessControlService.host | string | `"access-control:9006"` |  |
| accessControlService.secret | string | `"IC04LYMBf1lDP5oeY4hupxd4HJhLmN6azUku3xEbeE3SUx5G3ZYzhbiwVtK4i7AmqyU9OZkwB4v8E9qM"` |  |
| accessControlService.skipSecureVerify | string | `"true"` |  |
| affinity | object | `{}` |  |
| agent.customImage | string | `"true"` |  |
| agent.dockerImageRepo | string | `"harness/gitops-agent"` |  |
| agent.enableAuth | string | `"false"` |  |
| agent.minimumV2Version | string | `"0.33.0"` |  |
| agent.protocol | string | `"HTTP1"` |  |
| agent.tlsEnabled | string | `"false"` |  |
| agent.versionFileLocation | string | `"/app/VERSIONS/AGENT"` |  |
| agentDockerImage.image.digest | string | `""` |  |
| agentDockerImage.image.imagePullSecrets | list | `[]` |  |
| agentDockerImage.image.pullPolicy | string | `"Always"` |  |
| agentDockerImage.image.registry | string | `"docker.io"` |  |
| agentDockerImage.image.repository | string | `"harness/gitops-agent"` |  |
| agentDockerImage.image.tag | string | `"v0.42.0"` |  |
| agentHAProxyImage.image.digest | string | `""` |  |
| agentHAProxyImage.image.imagePullSecrets | list | `[]` |  |
| agentHAProxyImage.image.pullPolicy | string | `"IfNotPresent"` |  |
| agentHAProxyImage.image.registry | string | `"docker.io"` |  |
| agentHAProxyImage.image.repository | string | `"haproxy"` |  |
| agentHAProxyImage.image.tag | string | `"2.0.25-alpine"` |  |
| agentRedisImage.image.digest | string | `""` |  |
| agentRedisImage.image.imagePullSecrets | list | `[]` |  |
| agentRedisImage.image.pullPolicy | string | `"IfNotPresent"` |  |
| agentRedisImage.image.registry | string | `"docker.io"` |  |
| agentRedisImage.image.repository | string | `"redis"` |  |
| agentRedisImage.image.tag | string | `"6.2.6-alpine"` |  |
| argoAppSetImage.image.digest | string | `""` |  |
| argoAppSetImage.image.imagePullSecrets | list | `[]` |  |
| argoAppSetImage.image.pullPolicy | string | `"IfNotPresent"` |  |
| argoAppSetImage.image.registry | string | `"quay.io"` |  |
| argoAppSetImage.image.repository | string | `"argoproj/argocd-applicationset"` |  |
| argoAppSetImage.image.tag | string | `"v0.4.1"` |  |
| argoCDImage.image.digest | string | `""` |  |
| argoCDImage.image.imagePullSecrets | list | `[]` |  |
| argoCDImage.image.pullPolicy | string | `"IfNotPresent"` |  |
| argoCDImage.image.registry | string | `"quay.io"` |  |
| argoCDImage.image.repository | string | `"argoproj/argocd"` |  |
| argoCDImage.image.tag | string | `"v2.3.4"` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| certPath | string | `""` |  |
| enableCDN | string | `"false"` |  |
| eventsFrameworkEnvNamespace | string | `"free"` |  |
| fullnameOverride | string | `""` |  |
| gitopsHttpAcme | string | `"false"` |  |
| gitopsTaskLongPolling | string | `"true"` |  |
| global.ingress.enabled | bool | `false` |  |
| global.ingress.hosts[0] | string | `"my-host.example.org"` |  |
| global.ingress.objects.annotations | object | `{}` |  |
| global.ingress.tls.enabled | bool | `false` |  |
| global.ingress.tls.secretName | string | `"harness-ssl"` |  |
| global.internalIngress.enabled | bool | `false` |  |
| global.istio.enabled | bool | `false` |  |
| global.istio.gateway.create | bool | `false` |  |
| global.istio.virtualService.gateways | string | `nil` |  |
| global.istio.virtualService.hosts | string | `nil` |  |
| global.loadbalancerURL | string | `"https://test"` |  |
| grpcPort | int | `7909` |  |
| identitySecret | string | `"HVSKUYqD4e5Rxu12hFDdCJKGM64sxgEynvdDhaOHaTHhwwn0K4Ttr0uoOxSsEVYNrUU="` |  |
| image.digest | string | `""` |  |
| image.imagePullSecrets | list | `[]` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.registry | string | `"docker.io"` |  |
| image.repository | string | `"harness/gitops-service-signed"` |  |
| image.tag | string | `"v0.62.4"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.className | string | `"internal"` |  |
| ingress.hosts[0].host | string | `""` |  |
| ingress.hosts[0].paths[0].path | string | `"/gitops"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"ImplementationSpecific"` |  |
| jwtSecret | string | `"HVSKUYqD4e5Rxu12hFDdCJKGM64sxgEynvdDhaOHaTHhwwn0K4Ttr0uoOxSsEVYNrUU="` |  |
| keyPath | string | `""` |  |
| logFormat | string | `""` |  |
| metricsPort | int | `6565` |  |
| mongo.dbName | string | `"harness-gitops"` |  |
| mongo.dropAllIndexesOnce | string | `"false"` |  |
| mongo.enableReflection | string | `"true"` |  |
| mongo.password.key | string | `"mongodb-root-password"` |  |
| mongo.password.name | string | `"mongodb-replicaset-chart"` |  |
| mongo.username.key | string | `"mongodbUsername"` |  |
| mongo.username.name | string | `"harness-secrets"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| platformService.secret | string | `"IC04LYMBf1lDP5oeY4hupxd4HJhLmN6azUku3xEbeE3SUx5G3ZYzhbiwVtK4i7AmqyU9OZkwB4v8E9qM"` |  |
| platformService.skipSecureVerify | string | `"true"` |  |
| platformService.url | string | `"http://ng-manager:7090"` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| redis.masterName | string | `"harness-redis"` |  |
| redis.password.key | string | `"redisPassword"` |  |
| redis.password.name | string | `"harness-secrets"` |  |
| redis.sslCAPath | string | `""` |  |
| redis.sslEnabled | string | `"false"` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | int | `2` |  |
| resources.limits.memory | string | `"256Mi"` |  |
| resources.requests.cpu | int | `2` |  |
| resources.requests.memory | string | `"256Mi"` |  |
| securityContext | object | `{}` |  |
| service.grpcServerPort | int | `7909` |  |
| service.httpBind | string | `":7908"` |  |
| service.httpServerPort | int | `7908` |  |
| service.port | int | `80` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `"harness-default"` |  |
| timescale.certPath | string | `""` |  |
| timescale.dbName | string | `"harness_gitops"` |  |
| timescale.logLevel | int | `3` |  |
| timescale.password.key | string | `"timescaledbPostgresPassword"` |  |
| timescale.password.name | string | `"harness-secrets"` |  |
| timescale.useTls | string | `"false"` |  |
| tolerations | list | `[]` |  |
| upgraderImage.image.digest | string | `""` |  |
| upgraderImage.image.imagePullSecrets | list | `[]` |  |
| upgraderImage.image.pullPolicy | string | `"Always"` |  |
| upgraderImage.image.registry | string | `"docker.io"` |  |
| upgraderImage.image.repository | string | `"harness/upgrader"` |  |
| upgraderImage.image.tag | string | `"latest"` |  |
| versionFileLocation | string | `"/app/VERSIONS/SERVER"` |  |
| waitForInitContainer.image.digest | string | `""` |  |
| waitForInitContainer.image.imagePullSecrets | list | `[]` |  |
| waitForInitContainer.image.pullPolicy | string | `"IfNotPresent"` |  |
| waitForInitContainer.image.registry | string | `"docker.io"` |  |
| waitForInitContainer.image.repository | string | `"harness/helm-init-container"` |  |
| waitForInitContainer.image.tag | string | `"latest"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.0](https://github.com/norwoodj/helm-docs/releases/v1.11.0)
