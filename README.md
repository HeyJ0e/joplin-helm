# Joplin server

 [Joplin](https://joplinapp.org) is an open source note-taking app. [Joplin server](https://github.com/laurent22/joplin/tree/dev/packages/server) can be self-hosted to securely own and have full control on your data. This is an unofficial Helm Chart to install it on a Kubernetes cluster.

## Getting started

Add Helm repository

```bash
helm repo add joplin-server https://HeyJ0e.github.io/joplin-helm
helm repo update
```

Install

```bash
helm install joplin-server -n joplin-server joplin-server/joplin-server
```

## Customize

```bash
helm show values joplin-server/joplin-server > values.yaml
```

## Uninstall

```bash
helm delete joplin-server
helm repo remove joplin-server
```
