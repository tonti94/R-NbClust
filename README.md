# R-NbClust
How to use NbClust on R language
 data=iris
> data<-scale(iris[,-c(5)])
> pmatrix=scale(data)
> d=dist(pmatrix)
> c=hclust(d,method="ward.D2")
> library(NbClust)
> res.nb<-NbClust(pmatrix, min.nc=2,max.nc=10,method="complete")
