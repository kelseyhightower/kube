# kube

My repo for testing Kubernetes on a single GCP instance. The start up script provisions a Kubernetes 1.8 cluster with cri-containerd and Istio.

## Usage

Clone this repo and run the following commands:

Create a single node Kubernetes cluster:

```
./create-instance
```

Fetch the Kubernetes creds:

```
./get-credentials
```

Set the KUBECONFIG env var to use the `kube` credentials:

```
source kube.env
```

## Cleanup

```
./delete-instance
```
