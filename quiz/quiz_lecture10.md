# Quizzes for Lecture - 10

I added some comments at the end of the program that we just wrote today. If you can run the program, it will print some comments those comments will give you some hint about, why for 2 nodes, it did not give us correct result.
Also, further at the end, it will print your Quiz - 8!

And finally what if, I send you a file and ask, what does [this program](https://github.com/RupakMukherjee/fluid_teaching/blob/master/3d_hybrid_poisson.f95) do?
To compile and run this file, you may use the following command:
```console
 $ mpif90 -fopenmp -I/usr/local/include -L/usr/local/lib 3d_hybrid_poisson.f95 -lfftw3_mpi -lfftw3_omp -lfftw3 -lm; mpirun -quiet -np 3 ./a.out
```
### Quiz - 6: 
Can you turn the code [hybrid_do.f95] into a 3d hybrid Poisson solver?
If you can solve Quiz - 9, this course is over!!!

[Back to Lecture - 10](https://github.com/RupakMukherjee/fluid_teaching#lecture-10)
