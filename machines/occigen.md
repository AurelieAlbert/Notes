# All the tricks for occigen

## Conda environment with conda-pack

  - set-up the environment
    - on another linux machine (meom, cal1) :
       - set-up the conda environment normally (conda create, conda install)
       - conda install -c conda-forge conda-pack
       - conda pack -n my_env
    - on occigen, in /scratch/cnt0024/hmg2840/albert7a/DEV/git/conda-pack
       - mkdir -p my_env
       - tar -xzf my_env.tar.gz -C my_env
       - cond (add conda path to the PATH)
       - source my_env/bin/activate
       - python -m ipykernel install --user --name my_env --display-name my_env

  - use the environment
    - on occigen, in /scratch/cnt0024/hmg2840/albert7a/DEV/git/conda-pack
       - cond
       - source my_env/bin/activate
       - jupyter notebook, ipython or python
