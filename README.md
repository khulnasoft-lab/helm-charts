# KhulnaSoft Security Helm Charts

[![License][license-img]][license]

[license-img]: https://img.shields.io/badge/License-Apache%202.0-blue.svg
[license]: https://github.com/khulnasoft-lab/helm-charts/blob/master/LICENSE

KhulnaSoft Security Open Source Projects Helm Charts on a [Kubernetes](https://kubernetes.io) cluster using the
[Helm](https://helm.sh) package manager.

## Charts

- [Vul Operator](https://github.com/khulnasoft/vul-operator/tree/main/deploy/helm)
- [Starboard](https://github.com/khulnasoft-lab/starboard/tree/main/deploy/helm)
- [Vul](https://github.com/khulnasoft/vul/tree/main/helm/vul)
- [Postee](https://github.com/khulnasoft-lab/postee/tree/main/deploy/helm/postee)

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
helm repo add khulnasoft-lab https://khulnasoft-lab.github.io/helm-charts/
helm repo update
```

## Installing the Chart

Search all the repositories available
```
helm search repo khulnasoft-lab -l
```

Install specific helm chart
```
helm install starboard khulnasoft-lab/starboard-operator
helm status starboard
```

## Uninstalling the Chart

To uninstall/delete the `starboard` deployment:

```
$ helm delete starboard
```
