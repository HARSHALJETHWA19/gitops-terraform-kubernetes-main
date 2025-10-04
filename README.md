# GitOps Terraform EC2 mit KubeVela

Dieses Repository enthält die vollständige Konfiguration zur Bereitstellung einer EC2-Instanz mit einem Load Balancer über GitOps mit Flux und Terraform.

## Struktur
- `clusters/dev/` - Enthält die Flux-Konfigurationen.
- `terraform/` - Enthält die Terraform-Konfigurationsdateien.
- `manifests/` - Enthält Kubernetes-Manifeste für Flux.

## Installation

1. Installieren Sie Flux in Ihrem Kubernetes-Cluster.
2. Deployen Sie die Terraform-Ressourcen mit:

```bash
kubectl apply -f terraform/ec2-alb.yaml -n terraform
```
