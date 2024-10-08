# comfyui-on-gke

## build images
```shell
cd build/
cp Dockerfile.xxx Dockerfile
gcloud builds submit --region=us-west2 --tag gcr.io/PROJECT_ID/IMAGE_NAME .
```
