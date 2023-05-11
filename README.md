# sortingalgorithm_checkpoint
The steps taken are commented out as an algorthm
function insertionSort(arr){
    for(let i=1; i<arr.length; i++){  // loop through all elements of the array starting from index 1
      let current = arr[i];  // pick the current element to insert into the sorted sequence
      let j = i-1;           // initialize j as the index of the last element in the sorted sequence
      while(j>=0 && arr[j]>current){  // loop through the sorted sequence backwards
        arr[j+1] = arr[j];   // shift elements to the right to make space for the current element
        j--;                 // move j to the left
      }
      arr[j+1] = current;    // insert the current element into the sorted sequence
    }
    return arr;  // return the sorted array
  } 
