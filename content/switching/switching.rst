Switching
=========

Introduction
---------------
The time-integrated amount of data and stored information is doubled roughly every
18 months and, since the majority of the world’s information is stored in magnetic media,
the possibility writing and retrieving information in a magnetic material at ever greater
speed and with lower energy consumption has obvious benefits for our society. Hence,
the simple switching of a magnetic unit, a bit, is a crucial process which defines how efficiently information can be stored and retrieved from a magnetic memory. In the following exercises, you will use the code UppASD to perform magnetic switching simulation with several setups. Please find more simulation details in ``task.txt`` in each task folder.

Python environment for the GUI
------------------------------

The recommended way to set up the Python environment that is required
for the UppASD graphical user interface is to use either a Python
virtual environments or a conda environment.

First simulations
-----------------


UppASD on supercomputers
------------------------
The code is parallelized over shared memory using OpenMP threading. In this
exercise you will explore how the computational performance of UppASD depends
on problem size and on the number of CPU cores. With weak scaling is meant the
computational effiency when changing the number of cores in proportion with
the problem size. With strong scaling is meant the computational effiency when
changing the number of cores for a fixed problem size.

The systems

* Exercise 1: Weak scaling for ``NX 12``, ``NY 12``, ``NX 12``:math:`c`, where :math:`nc` is the number CPU cores, ranging from 1 to 16.

* Exercise 2: Strong scaling for ``NX 24``, ``NY 24``, ``NZ 24``, when varying the number of CPU cores :math:`nc` in the range from 1 to 16.
