# GRICAD 

 - account management : https://perseus.univ-grenoble-alpes.fr/
 - documentation : https://gricad-doc.univ-grenoble-alpes.fr/
 
 ## Login
 
  - from anywhere first : ssh -CX alberta@access-ciment.imag.fr or ssh -CX alberta@access-ciment.ujf-grenoble.fr
  - then ssh -CX dahu
  - procedure to avoid log in to the frontal first : https://gricad-doc.univ-grenoble-alpes.fr/hpc/connexion/
  
 ## Repos
 
   - /home/alberta for scripts
   - /bettik/alberta for data
   - mantis : ils -> /cigri/home/alberta
     - commandes irods : https://docs.irods.org/master/
     - iput
     
 ## Jobs
 
   - OAR syntax : https://oar.imag.fr/
   - oarsub, oarstat -u alberta
   
 ## Jupyterhub
 
   - directly : https://jupyterhub.u-ga.fr/hub/login with PERSEUS login and password -> no access to data
   - doc https://gricad-doc.univ-grenoble-alpes.fr/notebook/platform/
   
 ## Jupyter notebooks directly on clusters nodes
 
   - https://gricad-doc.univ-grenoble-alpes.fr/notebook/hpcnb/
   - for me the steps are :
    - login : ssh f-dahu.ciment
    - oarsub -I --project data-ocean -l /core=10,walltime=2:00:00
    - jupyter notebook
    - in a new terminal, ssh -fNL 8888:dahu78:8888 dahu.ciment
    - in chrome, http://localhost:8888/?token=0707924ea352afc4a19ff086a94266101a57e56754072340
    
 ## Nix : package managment
 
   - doc : https://gricad.github.io/calcul/nix/tuto/2017/07/04/nix-tutorial.html
   - install a package : nix-env -i python3.7-dask-2.10.1
   - list of all packages : nix-env -qaP | grep dask

