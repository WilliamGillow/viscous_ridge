# Convergent Viscous Gravity-Driven Flows

<div align="justify">

This serves as a companion to my fourth year project, containing useful items not found within the dissertation.

More specifically, this contains the code used to perform the numerical methods from my dissertation as well as to produce the snapshots from the comparison with direct numerical simulation (DNS) data. 
Furthermore, full animations can be found here too. In the code folder, this contains one subfolder for all of the numerics and one for the DNS comparisons.

The numerics folder has a file for each time scale in the Newtonian model and produces the plots seen in the numerics section. Variables such as the time interval, time step size, and the spatial mesh (so $N$ and $x_N$) can be modified
as desired in order to investigate behaviour of the fluid interface that is not directly displayed in the dissertation, although this covers the main features seen at each time scale. Upon changing variables, it is likely that axes scales 
and ticks will need to be changed too.

The file for the Bingham model is set up very similarly, although uses a different solver. In hindsight, it would have been best to use this throughout, but this only became apparent after I had written the code for the Newtonian model, 
and rewriting all of this would not have been an efficient use of my time. Again, variables can be modified in order to change the time frame, spatial mesh, but also now the Bingham number. This should be done cautiously as choosing to large 
a Bingham number, spatial step, time step, or too small a value of "nsteps" can lead to the solver failing to run until the end time due to the stiffness of the problem. Again, upon changing variables, it is likely that axes scales 
and ticks will need to be changed too.

The data from the DNS comparisons was generated using direct numerical simulation code written in the open-source [Basilisk](http://basilisk.fr/) software by one of my co-supervisors, [Dr. Radu Cimpeanu](https://github.com/RaduCimpeanu). Only the 
data for the snapshots is provided, so data would first need to be generated before being able to use the animation code, which may also require modification of the time interval and spatial domain for the asymptotic and numerical solutions 
depending on the data generated.

 </div>
