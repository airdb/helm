![Build Status](https://github.com/airdb/sailor/workflows/Go/badge.svg)

Helm Package Repo. [Heml index.yaml](/helm/index.yaml)

## Usage

```bash
helm repo add airdb https://www.airdb.com/helm/
helm repo update
helm search repo helm/mychart
helm install chart airdb/mychat
helm install chart airdb/mychat --dry-run --debug
```

## Helm V3 Profile

```bash
helm env
```

## Create or Update Helm Chart Repo

```bash
git clone https://github.com/airdb/helm/
cd helm
helm repo index ./ --url https://www.airdb.com/helm/

helm package mychart

Update the index.yaml file based on your chart.
cd helm
helm repo index --merge index.yaml --url https://www.airdb.com/helm/ .
```

## Other Repos

```bash
helm repo add stable https://kubernetes-charts.storage.googleapis.com
```
