# minio

![Version: 5.4.0](https://img.shields.io/badge/Version-5.4.0-informational?style=flat-square) ![AppVersion: RELEASE.2024-12-18T13-15-44Z](https://img.shields.io/badge/AppVersion-RELEASE.2024--12--18T13--15--44Z-informational?style=flat-square)

High Performance Object Storage

**Homepage:** <https://min.io>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| MinIO, Inc | <dev@minio.io> |  |

## Source Code

* <https://github.com/minio/minio>

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| additionalAnnotations | object | `{}` |  |
| additionalLabels | object | `{}` |  |
| affinity | object | `{}` |  |
| bucketRoot | string | `""` |  |
| buckets | list | `[]` |  |
| certsPath | string | `"/etc/minio/certs/"` |  |
| clusterDomain | string | `"cluster.local"` |  |
| configPathmc | string | `"/etc/minio/mc/"` |  |
| consoleIngress.annotations | object | `{}` |  |
| consoleIngress.enabled | bool | `false` |  |
| consoleIngress.hosts[0] | string | `"console.minio-example.local"` |  |
| consoleIngress.ingressClassName | string | `nil` |  |
| consoleIngress.labels | object | `{}` |  |
| consoleIngress.path | string | `"/"` |  |
| consoleIngress.tls | list | `[]` |  |
| consoleService.annotations | object | `{}` |  |
| consoleService.clusterIP | string | `nil` |  |
| consoleService.externalIPs | list | `[]` |  |
| consoleService.externalTrafficPolicy | string | `"Cluster"` |  |
| consoleService.loadBalancerIP | string | `nil` |  |
| consoleService.loadBalancerSourceRanges | list | `[]` |  |
| consoleService.nodePort | int | `32001` |  |
| consoleService.port | string | `"9001"` |  |
| consoleService.type | string | `"ClusterIP"` |  |
| containerSecurityContext.readOnlyRootFilesystem | bool | `false` |  |
| customCommandJob.exitCommand | string | `""` |  |
| customCommandJob.extraVolumeMounts | list | `[]` |  |
| customCommandJob.extraVolumes | list | `[]` |  |
| customCommandJob.resources.requests.memory | string | `"128Mi"` |  |
| customCommandJob.securityContext.enabled | bool | `false` |  |
| customCommandJob.securityContext.runAsGroup | int | `1000` |  |
| customCommandJob.securityContext.runAsUser | int | `1000` |  |
| customCommands | string | `nil` |  |
| deploymentUpdate.maxSurge | string | `"100%"` |  |
| deploymentUpdate.maxUnavailable | int | `0` |  |
| deploymentUpdate.type | string | `"RollingUpdate"` |  |
| drivesPerNode | int | `1` |  |
| environment | string | `nil` |  |
| etcd.clientCert | string | `""` |  |
| etcd.clientCertKey | string | `""` |  |
| etcd.corednsPathPrefix | string | `""` |  |
| etcd.endpoints | list | `[]` |  |
| etcd.pathPrefix | string | `""` |  |
| existingSecret | string | `""` |  |
| extraArgs | list | `[]` |  |
| extraContainers | list | `[]` |  |
| extraSecret | string | `nil` |  |
| extraVolumeMounts | list | `[]` |  |
| extraVolumes | list | `[]` |  |
| fullnameOverride | string | `""` |  |
| ignoreChartChecksums | bool | `false` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"quay.io/minio/minio"` |  |
| image.tag | string | `"RELEASE.2024-12-18T13-15-44Z"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0] | string | `"minio-example.local"` |  |
| ingress.ingressClassName | string | `nil` |  |
| ingress.labels | object | `{}` |  |
| ingress.path | string | `"/"` |  |
| ingress.tls | list | `[]` |  |
| makeBucketJob.exitCommand | string | `""` |  |
| makeBucketJob.resources.requests.memory | string | `"128Mi"` |  |
| makeBucketJob.securityContext.enabled | bool | `false` |  |
| makeBucketJob.securityContext.runAsGroup | int | `1000` |  |
| makeBucketJob.securityContext.runAsUser | int | `1000` |  |
| makePolicyJob.exitCommand | string | `""` |  |
| makePolicyJob.resources.requests.memory | string | `"128Mi"` |  |
| makePolicyJob.securityContext.enabled | bool | `false` |  |
| makePolicyJob.securityContext.runAsGroup | int | `1000` |  |
| makePolicyJob.securityContext.runAsUser | int | `1000` |  |
| makeServiceAccountJob.exitCommand | string | `""` |  |
| makeServiceAccountJob.resources.requests.memory | string | `"128Mi"` |  |
| makeServiceAccountJob.securityContext.enabled | bool | `false` |  |
| makeServiceAccountJob.securityContext.runAsGroup | int | `1000` |  |
| makeServiceAccountJob.securityContext.runAsUser | int | `1000` |  |
| makeUserJob.exitCommand | string | `""` |  |
| makeUserJob.resources.requests.memory | string | `"128Mi"` |  |
| makeUserJob.securityContext.enabled | bool | `false` |  |
| makeUserJob.securityContext.runAsGroup | int | `1000` |  |
| makeUserJob.securityContext.runAsUser | int | `1000` |  |
| mcImage.pullPolicy | string | `"IfNotPresent"` |  |
| mcImage.repository | string | `"quay.io/minio/mc"` |  |
| mcImage.tag | string | `"RELEASE.2024-11-21T17-21-54Z"` |  |
| metrics.serviceMonitor.additionalLabels | object | `{}` |  |
| metrics.serviceMonitor.annotations | object | `{}` |  |
| metrics.serviceMonitor.enabled | bool | `false` |  |
| metrics.serviceMonitor.includeNode | bool | `false` |  |
| metrics.serviceMonitor.interval | string | `nil` |  |
| metrics.serviceMonitor.namespace | string | `nil` |  |
| metrics.serviceMonitor.public | bool | `true` |  |
| metrics.serviceMonitor.relabelConfigs | object | `{}` |  |
| metrics.serviceMonitor.relabelConfigsCluster | object | `{}` |  |
| metrics.serviceMonitor.scrapeTimeout | string | `nil` |  |
| minioAPIPort | string | `"9000"` |  |
| minioConsolePort | string | `"9001"` |  |
| mode | string | `"distributed"` |  |
| mountPath | string | `"/export"` |  |
| nameOverride | string | `""` |  |
| networkPolicy.allowExternal | bool | `true` |  |
| networkPolicy.egressEntities[0] | string | `"kube-apiserver"` |  |
| networkPolicy.enabled | bool | `false` |  |
| networkPolicy.flavor | string | `"kubernetes"` |  |
| nodeSelector | object | `{}` |  |
| oidc.claimName | string | `"policy"` |  |
| oidc.claimPrefix | string | `""` |  |
| oidc.clientId | string | `"minio"` |  |
| oidc.clientSecret | string | `""` |  |
| oidc.comment | string | `""` |  |
| oidc.configUrl | string | `"https://identity-provider-url/.well-known/openid-configuration"` |  |
| oidc.displayName | string | `""` |  |
| oidc.enabled | bool | `false` |  |
| oidc.existingClientIdKey | string | `""` |  |
| oidc.existingClientSecretKey | string | `""` |  |
| oidc.existingClientSecretName | string | `""` |  |
| oidc.redirectUri | string | `"https://console-endpoint-url/oauth_callback"` |  |
| oidc.scopes | string | `"openid,profile,email"` |  |
| persistence.accessMode | string | `"ReadWriteOnce"` |  |
| persistence.annotations | object | `{}` |  |
| persistence.enabled | bool | `true` |  |
| persistence.existingClaim | string | `""` |  |
| persistence.size | string | `"500Gi"` |  |
| persistence.storageClass | string | `""` |  |
| persistence.subPath | string | `""` |  |
| persistence.volumeName | string | `""` |  |
| podAnnotations | object | `{}` |  |
| podDisruptionBudget.enabled | bool | `false` |  |
| podDisruptionBudget.maxUnavailable | int | `1` |  |
| podLabels | object | `{}` |  |
| policies | list | `[]` |  |
| pools | int | `1` |  |
| postJob.affinity | object | `{}` |  |
| postJob.annotations | object | `{}` |  |
| postJob.nodeSelector | object | `{}` |  |
| postJob.podAnnotations | object | `{}` |  |
| postJob.securityContext.enabled | bool | `false` |  |
| postJob.securityContext.fsGroup | int | `1000` |  |
| postJob.securityContext.runAsGroup | int | `1000` |  |
| postJob.securityContext.runAsUser | int | `1000` |  |
| postJob.tolerations | list | `[]` |  |
| priorityClassName | string | `""` |  |
| replicas | int | `16` |  |
| resources.requests.memory | string | `"16Gi"` |  |
| rootPassword | string | `""` |  |
| rootUser | string | `""` |  |
| runtimeClassName | string | `""` |  |
| securityContext.enabled | bool | `true` |  |
| securityContext.fsGroup | int | `1000` |  |
| securityContext.fsGroupChangePolicy | string | `"OnRootMismatch"` |  |
| securityContext.runAsGroup | int | `1000` |  |
| securityContext.runAsUser | int | `1000` |  |
| service.annotations | object | `{}` |  |
| service.clusterIP | string | `nil` |  |
| service.externalIPs | list | `[]` |  |
| service.externalTrafficPolicy | string | `"Cluster"` |  |
| service.loadBalancerIP | string | `nil` |  |
| service.loadBalancerSourceRanges | list | `[]` |  |
| service.nodePort | int | `32000` |  |
| service.port | string | `"9000"` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `"minio-sa"` |  |
| statefulSetUpdate.updateStrategy | string | `"RollingUpdate"` |  |
| svcaccts | list | `[]` |  |
| tls.certSecret | string | `""` |  |
| tls.enabled | bool | `false` |  |
| tls.privateKey | string | `"private.key"` |  |
| tls.publicCrt | string | `"public.crt"` |  |
| tolerations | list | `[]` |  |
| topologySpreadConstraints | list | `[]` |  |
| trustedCertsSecret | string | `""` |  |
| users[0].accessKey | string | `"console"` |  |
| users[0].policy | string | `"consoleAdmin"` |  |
| users[0].secretKey | string | `"console123"` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.14.2](https://github.com/norwoodj/helm-docs/releases/v1.14.2)
