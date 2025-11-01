# Cluster Addons

This directory contains the ArgoCD ApplicationSet and Helm chart for managing cluster addons across multiple clusters.

## Structure

- `addons-applicationset.yaml` - ArgoCD ApplicationSet for deploying addons to clusters
- `values-{cluster}.yaml` - Cluster-specific values files
- `cluster-config/{cluster}/config.json` - Cluster configuration files
- `templates/` - Helm chart templates

## Usage

The ApplicationSet uses the Git File Generator pattern to discover cluster configurations from `cluster-config/*/config.json` files.
