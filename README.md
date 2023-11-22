# Notes-for-Using-GPUs-with-Slurm

## Running Jobs

* submit jobs: ```sbatch job.sh```

* cancel jobs: ```scancel job.sh```

* list jobs: ```sq```

* output path: By default the output is placed in a file named "slurm-", suffixed with the job ID number and ".out" (e.g. ```slurm-123456.out```), in the directory from which the job was submitted.

* Check GPU usage on a node where you have a job running: ```srun --jobid JOB_ID --pty watch -n 10 nvidia-smi```

## Virtual Environments

Tutorial: [A Complete Guide for using Compute Canada for Deep Learning!](https://prashp.gitlab.io/post/compute-canada-tut/); [Creating and using a virtual environment](https://docs.alliancecan.ca/wiki/Python#Creating_and_using_a_virtual_environment)

* List available version: module avail xxx

1. Load Python: ```module load python/3.8```
2. Load other software (e.g. OpenCV): ```module load opencv/4.5.1```

* Create new environment: ```virtualenv --no-download test_env```

* Activate your environment: ```source ~/virtualenvs/test_env/bin/activate```

* Exit a virtual environment: ```deactivate```
