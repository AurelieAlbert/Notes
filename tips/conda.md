#Tips for conda

 - list the environment available for a machine : conda info --envs
 - make an environment for a machine with no http port : via conda-pack
    - on another machine with http port: 
      - create env with all the librairies needed and conda-pack (```conda install -c conda-forge conda-pack```)
      - ```conda pack -n env```
      - ```scp env.tar.gz``` to distant machine
    - on the distant machine :
      - ```tar -xzf env.tar.gz -C env```
      - ```source perf-pangeo/bin/activate```
