```
do i = 1,Nh
  kx = 2.0d0*pi*dfloat(i-1)/Lx
  do j = 1,Ny/2
    ky = 2.0d0*pi*dfloat(j-1)/Ly
    do k = 1,Nz/2
      kz = 2.0d0*pi*dfloat(k-1)/Lz 
      i_kx_omegak(i,j,k) = (0.0d0,1.0d0) * kx * omegak(i,j,k)
      i_ky_omegak(i,j,k) = (0.0d0,1.0d0) * ky * omegak(i,j,k)
      i_kz_omegak(i,j,k) = (0.0d0,1.0d0) * kz * omegak(i,j,k)      
    enddo
    do k = Nz/2+1,Nz
      kz = 2.0d0*pi*(dfloat(k-1)-Nz)/Lz
      i_kx_omegak(i,j,k) = (0.0d0,1.0d0) * kx * omegak(i,j,k)
      i_ky_omegak(i,j,k) = (0.0d0,1.0d0) * ky * omegak(i,j,k)
      i_kz_omegak(i,j,k) = (0.0d0,1.0d0) * kz * omegak(i,j,k)             
    enddo    
  do j = Ny/2+1,Ny
     ky = 2.0d0*pi*(dfloat(j-1)-Ny)/Ly
    do k = 1,Nz/2
      kz = 2.0d0*pi*dfloat(k-1)/Lz 
      i_kx_omegak(i,j,k) = (0.0d0,1.0d0) * kx * omegak(i,j,k)
      i_ky_omegak(i,j,k) = (0.0d0,1.0d0) * ky * omegak(i,j,k)
      i_kz_omegak(i,j,k) = (0.0d0,1.0d0) * kz * omegak(i,j,k)      
    enddo
    do k =  Nz/2+1,Nz
      kz = 2.0d0*pi*(dfloat(k-1)-Nz)/Lz
      i_kx_omegak(i,j,k) = (0.0d0,1.0d0) * kx * omegak(i,j,k)
      i_ky_omegak(i,j,k) = (0.0d0,1.0d0) * ky * omegak(i,j,k)
      i_kz_omegak(i,j,k) = (0.0d0,1.0d0) * kz * omegak(i,j,k)             
    enddo     
  enddo
enddo
```