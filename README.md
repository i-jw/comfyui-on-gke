# comfyui-on-gke

## build images
```shell
cd build/
cp Dockerfile.xxx Dockerfile
gcloud builds submit --region=us-west2 --tag gcr.io/PROJECT_ID/IMAGE_NAME .
```

## Install GPU Driver on GKE
```shell
kubectl apply -f https://raw.githubusercontent.com/GoogleCloudPlatform/container-engine-accelerators/master/nvidia-driver-installer/cos/daemonset-preloaded-latest.yaml
```
