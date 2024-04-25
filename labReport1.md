# Lab Report 1
## Isaac Chen PID: A17832849

**`ls`**
* No Arguments Given:
  * The absolute path before the command:
  * ![absPath](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/127a5080-36a8-44a9-b51c-d54c3c592c4e)
  * The command ran:
  * ![cmd](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/78f34f04-35e1-44c9-80f8-02a977817928)
  * Running `ls` without an arg results in it listing the current path we are at. In this case, it listed what is in `lecture1`. This is not an error.

* Directory as Path:
  * The absolute path before the command:
  * ![absPath](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/127a5080-36a8-44a9-b51c-d54c3c592c4e)
  * The command ran:
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/fbab420a-b737-429e-adf9-ee1fbc82f309)

  * Running `ls` with a directory as path results in it listing the files in the directory. In this case, it listed what is in `messages/`. This is not an error.
* File as Path:
  * The absolute path before the command:
  * ![absPath](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/127a5080-36a8-44a9-b51c-d54c3c592c4e)
  * The command ran:
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/06fb1f54-6d46-4e37-ba40-99f6cc01a0ca)
  * Running `ls` with a file as path results in it returning the file itself. In this case, it returned `Hello.java`. This is not an error.

***

**`cd`**
* No Arguments Given:
  * The absolute path before the command:
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/0f2b3a2a-9fa6-4e87-a073-af9b2d3bf6ac)
  * The command ran:
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/70bf6ff8-a494-40d9-bff7-825af37bfb32)
  * Running `cd` without an argument results in the directory changing to my home directory. This is not an error.
    
* Directory as Path:
  * The absolute path before the command:
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/f3db2677-c7e2-4156-881b-5d8cfb7b2593)
  * The command ran:
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/2558d394-1cf4-44bf-bff0-98982b144df8)
  * Running `cd` with a directory as path results in the directory changing to `messages/`. This is not an error.
    
* File as Path:
  * The absolute path before the command:
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/f3db2677-c7e2-4156-881b-5d8cfb7b2593)
  * The command ran:
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/1a4e095a-72d0-4eb6-a0bb-b7d787dd0ffe)
  * Running `cd` with a file as path results in the directory not changing becuase it's not a directory. This is an error because the given argument was invalid.

***

**`cat`**
* No Arguments Given:
  * The absolute path before the command:
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/ec6671e8-c3f7-4919-a058-bf2ca80ab730)
  * The command ran:
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/322979ac-7b03-4621-92f2-afda9d9b119d)
  * Running `cat` without an argument results in it returning the data's standard output. This is not an error.
    
* Directory as Path:
  * The absolute path before the command:
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/f3db2677-c7e2-4156-881b-5d8cfb7b2593)
  * The command ran:
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/c138ad18-3b7f-4be2-a521-478a31e922ff)
  * Running `cat` with a directory as path result in it returning that the arg is a directory. This is an error because `cat` can't be used on a directory.
    
* File as Path:
  * The absolute path before the command:
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/f3db2677-c7e2-4156-881b-5d8cfb7b2593)
  * The command ran:
  * ![image](https://github.com/JaysonKaleb/cse15l-lab-reports/assets/165828220/70234d06-3bf1-4648-99c7-b885825949d2)
  * Running `cat` with a file as path results in it returning the file's contents, i.e. `Hello.java`. This is not an error.

***
