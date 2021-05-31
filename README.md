# my_inverse_matrix
To find cache inverse matrix
 a <- makeCacheMatrix( matrix(c(5,6,7,8), nrow = 2, ncol = 2) );
> summary(a);
             Length Class  Mode    
setMatrix    1      -none- function
getMatrix    1      -none- function
cacheInverse 1      -none- function
getInverse   1      -none- function
> a$getMatrix();
     [,1] [,2]
[1,]    5    7
[2,]    6    8
> cacheSolve(a)
     [,1] [,2]
[1,]   -4  3.5
[2,]    3 -2.5
> cacheSolve(a)
getting cached data
     [,1] [,2]
[1,]   -4  3.5
[2,]    3 -2.5
> a <- makeCacheMatrix();
> summary(a);
             Length Class  Mode    
setMatrix    1      -none- function
getMatrix    1      -none- function
cacheInverse 1      -none- function
getInverse   1      -none- function
> a$setMatrix( matrix(c(5,6,7,8), nrow = 2, ncol = 2) );
> a$getMatrix();
     [,1] [,2]
[1,]    5    7
[2,]    6    8
> cacheSolve(a)
     [,1] [,2]
[1,]   -4  3.5
[2,]    3 -2.5
> cacheSolve(a)
getting cached data
     [,1] [,2]
[1,]   -4  3.5
[2,]    3 -2.5
> 
