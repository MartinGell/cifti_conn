# Brain-behaviour Predictions

This repository holds scripts to create `dconn` and `pconn` cifti files from `dtseries` or `ptseries` using data from s3 bucket that were preprocessed with xcpd. For any questions contact me @ martygell@gmail.com


<br />

The main script is in the `code` directory. Main additional processing options are:

1. Motion filtering
2. Outlier removal
3. Smoothing


<br />

Data from S3 will be loaded into the `input` directory and all processing will happen there. Therefore it is crucial to clone this directory into your own folder as no output paths are given - that is, this script operates within its own directory to improve reproducibility.


<br />


## Requirements:
1. Virtual environment
2. Access to s3 bucket
...

<br />

## 1. Environment
For this script to work a number of python modules are required. The easiest way to get these is using miniconda.

<br />

### Miniconda
In 'reqs' folder use the env_setup.yml to create the environemnt which will be called 'SNR':  
`conda env create -f (cloned_dir)/reqs/env_setup.yml`

Check env was installed correctly:  
`conda info --envs`

There should now be a ((miniconda_dir)/envs/SNR) visible

To activate env:  
`conda activate SNR`

References: https://medium.com/swlh/setting-up-a-conda-environment-in-less-than-5-minutes-e64d8fc338e4

<br />