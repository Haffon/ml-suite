# Jupyter Notebooks
The Jupyter Notebooks provide easy to use tutorials on how to use the xfDNN tools and deploy models within the Xilinx ML Suite.

## Installation 
1. Install Jupyter on the remote system (We recommend doing this inside your Anaconda environment). 
  ```
  $ source ~/.bashrc
  $ source activate ml-suite
  $ pip install jupyter`
  ```
  Follow the instructions to complete the install. You do not need to install Microsoft VScode, when prompted. 
  
2. Navigate to the top level `ml-suite' dir and source the setup script
  ```
  $ cd /ml-suite/
  $ source ./overlaybins/setup.sh <platform>
  ```
  Options for `<platform>`: `aws` `nimbix` `1525`

3. Set initial Password for Jupyter Server 
  ```
  $ jupyter notebook --generate-config
  $ jupyter notebook password 
  $ Enter Password: 
  $ Verify Password: 
  $ [NotebookPasswordApp] Wrote hashed password to /root/.jupyter/jupyter_notebook_config.json
  ```

## Launching Notebook Server 

1. Launch the jupyter notebook server  
  `jupyter notebook --no-browser --allow-root --ip=*`
  
2. On local machine, open a browser and navigate to `http://localhost:8888` or `youripaddress>:8888`

3. On a remote machine, open a browser on your local machine navigate to `yourpublicipaddress>:8888`
