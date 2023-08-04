![KhulnaSoft logo](https://avatars3.githubusercontent.com/u/12783832?s=200&v=4)
# KhulnaSoft Security Helm Charts

[![License][license-img]][license]

[license-img]: https://img.shields.io/badge/License-Apache%202.0-blue.svg
[license]: https://github.com/khulnasoft-labs/helm-charts/blob/master/LICENSE

KhulnaSoft Security Open Source Projects Helm Charts on a [Kubernetes](https://kubernetes.io) cluster using the
[Helm](https://helm.sh) package manager.

## Charts

- [Vul Operator](https://github.com/khulnasoft-labs/vul-operator/tree/main/deploy/helm)
- [Starboard](https://github.com/khulnasoft-labs/starboard/tree/main/deploy/helm)
- [Vul](https://github.com/khulnasoft-labs/vul/tree/main/helm/vul)
- [Postee](https://github.com/khulnasoft-labs/postee/tree/main/deploy/helm/postee)

## Prerequisites

- Kubernetes 1.15+ with Beta APIs enabled
- PV provisioner support in the underlying infrastructure

#### Installing [Helm](https://helm.sh)

```
curl -L https://git.io/get_helm.sh | bash
helm init
```

## Installing KhulnaSoft Community Helm Repository

```
helm repo add khulnasoft-labs https://khulnasoft-labs.github.io/helm-charts/
helm repo update
```

## Installing the Chart

Search all the repositories available
```
helm search repo khulnasoft-labs -l
```

Install specific helm chart
```
helm install starboard khulnasoft-labs/starboard-operator
helm status starboard
```

## Uninstalling the Chart

To uninstall/delete the `starboard` deployment:

```
$ helm delete starboard
```
