# Cluster Addons

This directory contains the ArgoCD ApplicationSet and Helm chart for managing cluster addons across multiple clusters.

## Structure

- `addons-applicationset.yaml` - ArgoCD ApplicationSet for deploying addons to clusters
- `cluster-config/{cluster}/config.json` - Cluster configuration files

## Usage

The ApplicationSet uses the Git File Generator pattern to discover cluster configurations from `cluster-config/*/config.json` files.
