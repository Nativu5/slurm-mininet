# Slurm in Mininet

This repo contains scripts for running Slurmd in virtual hosts of Mininet. 

The scripts is tested on Rocky Linux 9 and Slurm 23.11.

## Quick Start

1. Configure Slurmctld and Slurmdbd as usual. 

2. Make sure you have Mininet installed.

3. Run the following command to start Mininet with Slurmd in the virtual hosts:

```bash
sudo python3 launch.py
```

## Configuration

This repo contains sample slurm configurations. For slurmd, `slurm-mininet.conf` is used. Please be noticed that the slurmctld should be configured correspondingly.

Besides, `benchmark.yaml` is provided for running this repo in a cluster. You can modify the `benchmark.yaml` to fit your own cluster.

If no `benchmark.yaml` is provided, you can use CLI to configure. Please use `--help` to see the available options.
