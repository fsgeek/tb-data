# Tinymembench data

This is data that I have collected from a variety of source machines.

## March 3, 2021

First "serious" runs.  I collected data from three different machines:

* The AEP machine (Intel dual node system with 512GB PMEM modules)
* The NUC machine (Intel single node lightweight system)
* A VM on my desktop system (AMD Ryzen 3990X, 16 logical cores in the local machine)
* A dedicated (2 core) bare metal VM (Linode) using AMD EPYC 7501.

For the AEP machine, I used numactl to bind to a single core in the "local" node for the PMEM.
For all three, I ran as root, which causes the FIFO scheduler to be used, so it minimizes context switches.

The results are certainly interesting...
