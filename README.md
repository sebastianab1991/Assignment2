# Assignment2

## Creates a special matrix object that can cache its inverse
makeCacheMatrix <- function( m = matrix() ) {

	## Initialize the inverse property
    i <- NULL
    set <- function( matrix ) {
            m <<- matrix
            i <<- NULL
    }
    get <- function() {
    	m
    }
    setInverse <- function(inverse) {
        i <<- inverse
    }
    getInverse <- function() {
        i
    }
    list(set = set, get = get,
         setInverse = setInverse,
         getInverse = getInverse)
}
