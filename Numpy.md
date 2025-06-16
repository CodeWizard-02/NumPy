1. NumPy Introduction :-
	1. NumPy is a python library for arrays calculation and manipulation
	2. It is originally written in C for fast compilation
	3. C is the main reason, as it is way more faster than normal python lists

2. NumPy Arrays :-
	1. NumPy arrays are similar to python lists, but can store same datatype, whereas in lists, Mixed datatypes are allowed
	2. NumPy arrays are much more faster than traditional python lists, because it is written in C language
	3. Vector operations are easy and fast, compared to lists
	4. NumPy arrays support multi-dimensional lists, but lists doesn't support multi-dimensions

3. NumPy Arrays creation functions :-
	1. np.array() : creates an array

4. NumPy Arrays generation function :-
	1. np.arange(start, end) : creates arrays from start value to end value
	2. np.zeroes(value) : creates vector array of zeroes
	3. np.zeroes((rows, columns)) : creates a matrix of zeroes
	4. np.ones(value) : creates a vector of ones
	5. np.ones((rows, columns)) : creates a matrix of ones
	6. np.linspace(start, stop, no.of.elements) : creates an array of equally spaced

5. NumPy Arrays random generation functions :-
	1. np.random.rand(value) : creates random vector of elements(normalized {0-1})
	2. np.random.randn(value) : creates random vector of elements(standardized {3-(-3)})
	3. np.random.randint(6) : generate single random integer from 0-6
	4. np.random.randint(start, end, no.of.elements) : generate random integers between start and end

6. NumPy Array attributes :-
	1. arr.shape : no of rows and columns
	2. arr.size : no of elements
	3. arr.dtype : datatype of array

7. NumPy Array methods :-
	1. arr.min() : minimum value of array
	2. arr.max() : maximum value of array 
	3. arr.sum() : sum of all elements in array
	4. np.sum(arr, axis = 0/1) : sum elements row wise or columns wise {0 for columns and 1 for rows}
	5. arr.mean() : returns mean of the array
	6. arr.std() : returns standard deviation of the array
	7. arr.argmax() : returns index value of the max element
	8. arr.argmin() : returns index value of the min element
	9. arr.reshape(rows, columns) : returns the reshape matrix. Remember the no of rows and columns should be equal to number of elements

8. NumPy Array Indexing and Slicing :-
	1. arr[index] : returns the value of the index
	2. arr[startIndex:endIndex+1] : returns a range of values 
	3. arr[:endIndex+1] : returns range from index 0 to end value
	4. arr[startIndex:] : returns range from start value to last index
	5. arr[startIndex::steps] : returns range of values from start with gaps(steps)
	6. arr[rowIndex] : returns the indexed row of the matrix
	7. arr[rowIndex, columnIndex] : returns the elements of the selected rows and columns
	8. arr[rowIndex1:rowIndex2, columnIndex1:columnInde2] : returns the portion of the sliced matrix
	9. arr[:,columnIndex] : returns the column of a matrix

9. NumPy Array operations :-
	1. arr % 2 == 0 : returns True or False in the array itself(example of boolean indexing). After assigning it in arr it will remove the False values
	2. arr1 + arr2 : returns the sum of two arrays. Note: size of both the arrays must be same
	3. arr1 - arr2 : returns the sub of two arrays
	4. arr1 * arr2 : returns the product of two arrays
	5. arr1 / arr2 : returns the division of arrays
	6. arr1 // arr2 : returns the floor value of arrays
	7. arr1 ** arr2 : returns the exponential values of arrays
	8. arr + 10 : returns the +10 no of elements should be same added value by Broadcasting. Because adding values in existing values is not possible in lists

10. NumPy Matrix operations :-
	1. arr1 @ arr2 : returns the values of rows multiplied by columns. Also called as Dot Product Multiplication
	2. np.dot(arr1, arr2) : returns the dot products values
	3. arr.T : returns the transpose of the matrix

11. Array Stack and Splitting :-
	1. np.vstack() : returns the vertically stacked of arrays. Note: Stacking is not possible in matrix as it is already stacked
	2. np.hstack() : returns the horizontally stacked of arrays
	3. np.column_stack() : returns the columned stacked of arrays
	4. np.hsplit(arr, no.of.splits) : returns the horizontal split of matrix
	5. np.vsplit(arr, no.of.splits) : returns the vertical split of matrix