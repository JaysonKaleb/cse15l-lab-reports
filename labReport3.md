# Lab Report 39
## Isaac Chen Pid: A17832849

**Part 1**

***

* `ArrayExamples reversed Method`
  * Failure-Inducing Output
  ```
  @Test
  public void testReversed() {
    int[] input1 = {1,2,3};
    assertArrayEquals(new int[]{3,2,1 }, ArrayExamples.reversed(input1));
  }
  ```
  * Success-Inducing Output
  ```
	@Test 
	public void reversedEmpty() {
    int[] input1 = {  };
    ArrayExamples.reversed(input1);
    assertArrayEquals(new int[]{  }, input1);
	}
  ```
  * Symptom
    * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/1b78e32e-2546-4353-a917-179d06decd16)

  *`The Bug`
    * `Before`
      ```
      static int[] reversed(int[] arr) {
      	int[] newArray = new int[arr.length];
      	for(int i = 0; i < arr.length; i += 1) {
      		arr[i] = newArray[arr.length - i - 1];
      	}
      	return arr;
      }
      ```
    * `After`
      ```
      static int[] reversed(int[] arr) {
    	int[] newArray = new int[arr.length];
    	for(int i = 0; i < arr.length; i += 1) {
     	 newArray[i] = arr[arr.length - i - 1];
      	}
       return newArray;
      }
      ```
    * `Running Tests`
        ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/1bef34a2-cfc7-4475-a78c-8c90b5677861)
     
  
    * `Explanation`
      * First, the method originally returned arr which is just the given array, not the reversed array. Second of all, the for loop that reversed the array had 
         arr and newArray incorrectly swapped, resulting in it always copying zero. Thus, I changed the return to newArray, and swapped the two arrays in the for-loop.



**Part 2**

***

***
