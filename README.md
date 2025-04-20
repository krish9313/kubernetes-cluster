📝 Short Note: Deploying NGINX on Local Kubernetes with KIND

This guide demonstrates how to set up a local Kubernetes cluster using KIND (Kubernetes IN Docker) and deploy an NGINX web server.

🔧 Setup Steps:
      Clone Repo
      git clone https://github.com/vivekdalsaniya12/kubernetes-kind.git

Install Tools

    kubectl – Kubernetes CLI tool

kind – Tool to run Kubernetes clusters in Docker

Create Cluster

Use cluster.yml config to create a cluster

Verify with kubectl cluster-info

Repo Files

nginx-deployment.yaml: Deploys 3 replicas of NGINX

nginx-service.yaml: Exposes NGINX via NodePort 30001

Deploy

Apply the YAML files using kubectl apply

Verify Setup

Check nodes, pods, and services with kubectl get commands

Access NGINX via http://localhost:30001

Clean Up

Delete resources with kubectl delete -f .
