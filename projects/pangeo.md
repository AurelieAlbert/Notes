# PANGEO deployments 

## Les données eNATL60/NATL60 sur le cloud

### Inventaire des zarrs au 24 mars 2020

#### Sur le cloud
  - NATL60-CJM165-SSH-1h-1m2deg2deg/
  - NATL60-CJM165-SSH-1h-2D
  - NATL60-CJM165-SSU-1h-1m2deg2deg
  - NATL60-CJM165-SSV-1h-1m2deg2deg
  - eNATL60-BLB002-SSU-1h
  - eNATL60-BLB002-SSV-1h
  - eNATL60-BLBT02-SSU-1h
  - eNATL60-BLBT02-SSV-1h
  - eNATL60-BLBT02X-ssh
  - eNATL60-I
  - eORCA025-I
  - eORCA1-I
  - zarr-eNATL60, avec zarr_eNATL60-BLB002-SSU-1h-y2009m07-09 y2010m01-03 dedans
  - zarr_NATL60-CJM165_SSU_1h_y2013m07-09
    
  
#### Sur cal1
  - eORCA025 : /mnt/meom/workdir/albert/eORCA025/zarr_mesh_mask_eORCA025
  - eORCA1 : /mnt/meom/workdir/albert/eORCA1/zarr_IPSLCM6ALR_eORCA1.2_mesh_mask
  - in /mnt/meom/workdir/albert/eNATL60/zarr :
    - eNATL60-BLB002-SSU-1h
    - eNATL60-BLBT02-SSH-1h
    - eNATL60-BLBT02-SSU-1h
    - eNATL60-BLBT02-SSV-1h
    
#### Sur occigen
  - /store/albert7a/eNATL60/zarr :
   - eNATL60-BLB002-SSH-1h
   - eNATL60-BLB002X-SSH-1h
   - eNATL60-BLB002X-SSH-1h-bis
   - eNATL60-BLBT02-SSH-1h
   
#### Check si zarr ok
 
 https://github.com/auraoupa/zarr-check-all-platforms

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
