
Description
===========

Collection of ansible playbooks to deploy virtual elastic clusters in cloud infrastructures.

It includes playbooks to install:
- SLURM 2.5.7: used to work with pyslurm
- Pyslurm that works with SLURM 2.5.X
- NFS
- BLCR 0.8.5

Usage
=====

In the "Worker Nodes":
```yml 
roles:
    - { role: 'amcaar.slurm', slurm_type_of_node: 'wn', cloud: 'one'}
```
In the "Front-end node":
```yml
roles:
    - { role: 'amcaar.slurm', slurm_type_of_node: 'front', cloud: 'ec2'}
```

Note: the 'cloud' parameter specifies the provider of cloud computing resources that you want to use (by default, it is used 'one')

