
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
    - { role: 'amcaar.slurm', slurm_type_of_node: 'wn'}
```
In the "Front-end node":

```yml
roles:
    - { role: 'amcaar.slurm', slurm_type_of_node: 'front'}
```


