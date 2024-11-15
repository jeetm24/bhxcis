A <- matrix(c(1, 2, 3, 4, 5, 6), nrow = 2, ncol = 3, byrow = TRUE)
print(paste("Original Matrix:"))
print(A)

mean_A <- mean(as.vector(A))
print(paste("Mean of the Matrix:"))
print(mean_A)

if (det(A) != 0) {
  inverse_A <- solve(A)
  print(paste("Inverse of the Matrix:"))
  print(inverse_A)
} else {
  print("Matrix is singular and cannot be inverted.")
}
