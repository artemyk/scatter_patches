scatter_patches
===============

MATLAB function to generate scatter plots using patch objects

For a simple example, run:
```matlab
scatter_patches(randn(100,1),randn(100,1),'r','FaceAlpha',0.3,'EdgeColor','none');
```

For a more sophisticated example, run:
```matlab
N=100;
hh1=scatter_patches(randn(N,1),1*randn(N,1),36, 'r','FaceAlpha',0.4,'EdgeColor','none');
hold on;
hh2=scatter_patches(randn(N,1),2*randn(N,1),36, N*rand(N,1),'s','FaceAlpha',0.2,'EdgeColor','none');
hold on;
hh3=scatter_patches(randn(N,1),4 + 1*randn(N,1),100*rand(N,1), 1:N,'<','FaceAlpha',0.2,'EdgeColor','r');
legend([hh1(1),hh2(1),hh3(1)], {'red circles','multicolor squares','multicolor triangles'});
```
