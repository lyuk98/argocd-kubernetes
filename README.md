# Argo CD Applications

This repository contains Kustomizations that Argo CD Applications use to set up my personal Kubernetes cluster. The following resources are present:

- Argo CD
  - HTTPRoute and GRPCRoute for accessing Argo CD via Gateway API
- cert-manager
  - ClusterIssuer for issuing certificates from Let's Encrypt (both production and staging servers)
- Tailscale
  - Cilium configuration to use Tailscale as its LoadBalancer
  - GatewayClass and Gateway resources

Further configuration for the cluster can be found [on a separate repository](https://github.com/lyuk98/opentofu-kubernetes) for OpenTofu.
