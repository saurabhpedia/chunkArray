# DataChunkArray

This function creates an array of elements split into groups of the given size. If the input array cannot be split evenly, the final chunk will contain the remaining elements.

## Usage

```javascript
const chunkArray = require('./chunkArray');

const inputArray = ['a', 'b', 'c', 'd'];
const chunkSize = 2;
const output = chunkArray(inputArray, chunkSize);
console.log(output);
````


## Parameters
`array` (Array): The input array to be chunked.
`size` (number): The size of each chunk.


### Return Value
(Array): An array of chunks, where each chunk contains size number of elements from the input array. If the input array cannot be split evenly, the final chunk will contain the remaining elements.

The splice() method is used to extract elements from the original array (arr) starting from index 0 up to the given size. This creates a chunk of elements that is pushed into the result array. The splice() method also removes the extracted elements from the original array. This process continues until the original array is empty.