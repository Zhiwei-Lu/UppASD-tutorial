Switching
=========

Introduction
---------------
The time-integrated amount of data and stored information is doubled roughly every
18 months and, since the majority of the world’s information is stored in magnetic media,
the possibility writing and retrieving information in a magnetic material at ever greater
speed and with lower energy consumption has obvious benefits for our society. Hence,
the simple switching of a magnetic unit, a bit, is a crucial process which defines how efficiently information can be stored and retrieved from a magnetic memory. In the following exercises, you will use the code UppASD to perform magnetic switching simulation with several setups. Please find more simulation details in ``task.txt`` in each task folder.


TASK1
-----------------
The magnetization direction of sample can be manipulated by applying an external magnetic field with the desired orientation. In this exercise you will apply a magnetic field to switch the magnetization direction of bcc Fe from **+z** to **-z** direction. Set the flag ``hfield`` to turn on the magnetic field. Plot the average magnetization of **z** component as a function of time, compare the switching time of different strength with the magnetic field.

TASK2
------------------------
Damping enters the LLG equation as a phenomenological term, which denotes the energy and angular momentum dissipation from the magnetic system to the environment. The magnetic switching is heavily dependent on the damping. In this exercise you can modify the damping of system by the flag ``damping``, fix the magnetic field and compare the switching time of bcc Fe with different damping. 

TASK3
------------------------
To switch a magnetic system, one needs to overcome the energy barrier, which is determined by system’s magnetic anisotropy and the volume of the system. In actual device, the energy barrier can stablize system's magnetic order. However, huge energy barrier will induce higher power consumption to manipulate the magnetism in device. In this assignment, you will explore the magnetic switching process with different magnetic anisotropy and cell size. 
* Use the flag ``anisotropy`` combined with an external file storing the magnetic anisotropy parameter of system to manipulate the magnetic anisotropy, compare how different magnetic anisotropy affects the switching time.\\
* Use the flag ``ncell`` to control the size of system. Does the switching time increase with larger cell size? If not, can you explain it? 
The systems

* Exercise 1: Weak scaling for ``NX 12``, ``NY 12``, ``NX 12``:math:`c`, where :math:`nc` is the number CPU cores, ranging from 1 to 16.

* Exercise 2: Strong scaling for ``NX 24``, ``NY 24``, ``NZ 24``, when varying the number of CPU cores :math:`nc` in the range from 1 to 16.
