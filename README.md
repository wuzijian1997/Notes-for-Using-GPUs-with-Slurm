# Notes-for-Using-GPUs-with-Slurm

## Running Jobs

* submit jobs: ```sbatch job.sh```

* cancel jobs: ```scancel job.sh```

* list jobs: ```sq```

* output path: By default the output is placed in a file named "slurm-", suffixed with the job ID number and ".out" (e.g. ```slurm-123456.out```), in the directory from which the job was submitted.

## Virtual Environments

* List available version: module avail xxx

1. Load Python: ```module load python/3.10```
2. Load other software (e.g. OpenCV): ```module load opencv/4.5.1```
