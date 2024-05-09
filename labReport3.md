# Lab Report 3
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
* `less`
    * Display Line Numbers `-N`
      ```
      $ less -N biomed
      biomed is a directory
      ```

      ```
      $ less -N journal.pbio.0020001.txt
        1
      2
      3
      4
      5
      6         Kofi Annan, the Secretary-General of the United Nations, recently called attention to
      7         the clear inequalities in science between developing and developed countries and to the
      8         challenges of building bridges across these gaps that should bring the United Nations and
      9         the world scientific community closer to each other (Annan 2003). Mr. Annan stressed the
      10         importance of reducing the inequalities in science between developed and developing
      11         countries, asserting that “This unbalanced distribution of scientific activity generates
      12         serious problems not only for the scientific community in the developing countries, but for
      13         development itself.” Indeed, Mr. Annan's sentiments have also been echoed recently by
      14         several scientists, who present overwhelming evidence for the disparity in scientific
      15         output between the developing and already developed countries (Gibbs 1995; May 1997;
      16         Goldemberg 1998; Riddoch 2000). For example, recent United Nations Educational, Scientific,
      17         and Cultural Organization (UNESCO) estimates (UNESCO 2001) indicate that, in 1997, the
      18         developed countries accounted for some 84% of the global investment in scientific research
      19         and development, had approximately 72% of the world researchers, and produced approximately
      20         88% of all scientific and technical publications registered by the Science Citation Index
      21         (SCI). North America and Europe clearly dominate the number of scientific publications
      22         produced annually, with 36.6% and 37.5%, respectively, worldwide (UNESCO 2001).
      23
      24
      25             North America and Europe clearly dominate the number of scientific
      26             publications produced annually.
      27
      28
      29         It is rather obvious that richer countries are able to invest more resources in science
      ```
       * `-N` can be useful to find the exact line of a file while using less.
    * Leave File Contents `-X`
      ```
      $ less -X biomed
      biomed is a directory 
      ```
      
      ```
      $ less -X \1468-6708-3-1.txt




        Introduction
        Older adults are frequently counseled to lose weight,
        even though there is little evidence that overweight is
        associated with increased mortality in those over age 65.
        Six large controlled population-based studies of
        non-smoking older adults have investigated the association
        between body mass index (BMI) and mortality, controlling
        for relevant covariates [ 1 2 3 4 5 6 ] . All studies found
        excess risk for persons with very low BMI, but that persons
        with moderately high BMI had little or no extra risk except
        in certain small subsets. A review of 13 studies of older
        adults drew similar conclusions [ 7 ] .
        Many healthy older adults report gradual weight gain
        throughout adult life. It may be that a small amount of
        gradual weight gain is normative and associated with the
        most robust health as we age. It has been suggested that
        weight standards be adjusted upwards for age [ 8 ] . Such
        recommendations remain controversial, however, because the
        number of studies of older persons is fairly small, and
        because few studies have examined the relation of BMI to
        quality of life or years of healthy life (YHL) in the
        elderly [ 9 ] .
        In older adults, risk factors may have a greater effect
        on health than on mortality. If so, then behavior change
        trials of weight modification might be more successful if

      Jayso@MSI MINGW64 ~/CSE 15L/docsearch/technical/biomed (main)
      $
      ```
      * -X can be useful when you want to still look at the file's contents while being able to still use the terminal for the next command.

* Source: [https://linuxize.com/post/less-command-in-linux/](https://linuxize.com/post/less-command-in-linux/)
