# PANGEO deployments 

## Les données eNATL60/NATL60 sur le cloud

### Inventaire des zarrs au 24 mars 2020

#### Sur le cloud

#### Sur cal1

#### Sur occigen


### Pour la conversion en zarr

 - https://github.com/auraoupa/make-zarr-occigen

#### Ressources

 - https://github.com/pangeo-data/pangeo-datastore/issues/8

### Les commandes liées au cloud

  - gcloud auth login
  - gcloud init : mon projet est pangeo-181919, la région est US-CENTRAL1
  - gsutil -u pangeo-181919 ls -a gs://pangeo-meom
  - gsutil -m scp -r albert7a@occigen.cines.fr:/store/albert7a/NATL60/NATL60-CJM165-S/1h/SSH/NATL60-CJM165-SSH-1h gs://pangeo-data/

#### Ressources

[Google Cloud Platform](https://console.cloud.google.com/storage/browser/pangeo-data/)

[Cleaning out the pangeo-data google cloud storage bucket - Cloud - Pangeo](https://discourse.pangeo.io/t/cleaning-out-the-pangeo-data-google-cloud-storage-bucket/353)

[ocean: Pangeo Oceanography Dataset Catalog — Pangeo Catalog  documentation](https://pangeo-data.github.io/pangeo-datastore/master/ocean.html)

[GitHub - pangeo-data/pangeo-datastore: Pangeo Cloud Datastore](https://github.com/pangeo-data/pangeo-datastore)

[auraoupa/pangeo-data-catalog · GitHub](https://github.com/auraoupa/pangeo-data-catalog.git)

file:///Users/auraoupa/Downloads/Brodeau-LeSommer_ocean-modelling-splinter_SWOT-ST-2019.pdf
