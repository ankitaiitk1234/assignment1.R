# assignment1.R
# Solution of Assignment1.R
tennis <- function(p)
{
  x <- p*4
  y <- (1-p)*4
  if((x) >(y)){
  
  return(x)
  } else {
  return(y)
  }
}
tennis(4)

#
games <- numeric(1000)

for(i in 1:1000)
{
  games[i] <- tennis(3)
}
ans <- mean(games)
