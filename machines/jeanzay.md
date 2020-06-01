# Working on Jean Zay

 - mon login : rote001
 - mon mdp : lil-date
 - projet Melody : 101030
 - projet JMB et Stephanie : A0060101279
 - me logguer from meom : ssh -CX rote001@jean-zay.idris.fr
 
## Gestion des projets

  - mes projets : idrproj
    - egi :JMB et Stéphanie
    - yrf : Melody
    - ote : Drakkar ?
  - changer de projet actif : idrproj -d grp1
 
## Faire tourner le serveur jupyterhub

   - ssh to cal1, ssh meom, ssh -CY rote001@jean-zay.idris.fr
   - module load python
   - salloc --ntasks=1 --cpus-per-task=5 --account=egi@cpu --time=00:10:00 srun --pty bash
   - idrlab or idrjup, --notebook-dir=$WORK
   - on local machine, ssh -ND 3128 alberta@ige-meom-cal1.u-ga.fr
   - in the firefox browser parameters/advanced/ set up a proxy : SOCKS, server name = localhost, port 3128

 
### Ressources
 
  - http://www.idris.fr/eng/jean-zay/cpu/jean-zay-cpu-calculateurs-disques-eng.html
  - http://www.idris.fr/jean-zay/cpu/jean-zay-cpu-doc_multi_projet.html
  - http://www.idris.fr/jean-zay/pre-post/jean-zay-jupyter-notebook.html
  
