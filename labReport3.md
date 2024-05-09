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




**Part 2**

***
* `cat` Private Key
  * ![Screenshot 2024-04-16 151610](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/a1c91e07-4e07-4e8c-9d9c-ef0bc3934f6d)

* `cat` Public Key
  * ![Screenshot 2024-04-16 151713](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/f128a388-48ad-4133-b0a2-d7e807581ad1)

* Log-in Without Password 
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/9e4900cb-9877-4e19-b788-bea8eff0727e)


**Part 3**

***
Something new I learned from week 2 & 3 was how to use the cmd `curl` to access URLs. This was useful during Skill Demo 1 when our browsers were locked.
