# iot-p3-rcaillie — GitOps application manifests

Kubernetes manifests (`deployment`, `service`, `ingress`) for a sample web app,
deployed **continuously by Argo CD** in the Part 3 of my
[Inception-of-Things](https://github.com/rom98759/Inception-of-Things) École 42
project (K3s + K3d + Argo CD GitOps).

This repository is intentionally minimal: it is the **source of truth** that the
Argo CD `Application` watches. Any change pushed here is automatically synced to
the cluster.

## Contenu

| Fichier | Rôle |
|---|---|
| `deployment.yaml` | Déploiement de l'application (réplicas, image) |
| `service.yaml` | Service ClusterIP exposant les pods |
| `ingress.yaml` | Règle d'entrée HTTP |

Voir le dépôt [Inception-of-Things](https://github.com/rom98759/Inception-of-Things)
pour l'infrastructure complète et la configuration Argo CD.
