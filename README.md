# Notes-for-Using-GPUs-with-Slurm

submit jobs: ```sbatch job.sh```

cancel jobs: ```scancel job.sh```

list jobs: ```sq```

output path: By default the output is placed in a file named "slurm-", suffixed with the job ID number and ".out" (e.g. ```slurm-123456.out```), in the directory from which the job was submitted.
