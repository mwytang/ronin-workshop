Building a HPC Cluster
==================

Exercise 3: Build a HPC Cluster
-------------------------------
**Objectives**

#. Build an Auto-Scaling HPC Cluster
#. Connect to the HPC Cluster
#. Submit jobs to the HPC Cluster

**Configuration**

* **Operating System:** Ubuntu 18.04
*	**Scheduler:** Slurm scheduler
*	**Name:** my-windows-NAME or INITIAL – e.g., my-cluster-JohnSmith, my-cluster-JS
*	**Compute Node:** t3.medium
*	**Compute Nodes:** Min: 1; Max: 25
*	**SSH Key:** Key generated from Exercise 2

**Stress the HPC Cluster**

.. code-block:: console

   $ cd /apps/
   $ spack install stress
   $ vim stress.sh

.. code-block:: bash

   #!/bin/bash
   #SBATCH --nodes=1
   #SBATCH --ntasks-per-node=1
   spack load stress
   stress --cpu 2 --timeout 300s --verbose

.. code-block:: console

   $ chmod +x stress.sh
   $ squeue
   $ sbatch -a [1-10] stress.sh
   $ sbatch -a [1-15] stress.sh

**Referrences**

* **Instructions:** https://blog.ronin.cloud/auto-scale-a-cluster/
* **Simple Slurm Guide:** https://blog.ronin.cloud/slurm-intro/
* **Ganglia Guide:** https://blog.ronin.cloud/ganglia/ 
