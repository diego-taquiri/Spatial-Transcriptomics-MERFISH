# download merfish dataset 

https://info.vizgen.com/mouse-brain-map

curl https://sdk.cloud.google.com | bash
exec -l $SHELL
gcloud init

gcloud auth login

gsutil -m cp -r \
  "gs://public-datasets-vizgen-merfish/datasets/mouse_brain_map/BrainReceptorShowcase/Slice2/Replicate3/images" \
  .