###### CS-207-3: Programming II <br> Spring 2021 <br> Northeastern Illinois University <br> HW01-Review <br> Methods and Conditionals

**Getting Started**

**1.** Go to File > Project Structure. Under Project Settings, click on Project and verify that 
the Project SDK is set to JDK 11 or higher.  If it is not, select the correct SDK from the drop-down.<br>
**2.** Go to File > Settings (Mac: IntelliJ IDEA > Preferences). Under Build, Execution, Deployment 
and under Build Tools, click Gradle. Make sure Build and run using: and Run tests using: are set to 
Gradle. Make sure Use Gradle from: is set to 'gradle-wrapper.properties' file. And make sure Gradle 
JVM is set to JDK 11 or higher.<br>
**3.** Project SDK and Gradle JVM should be set to the same Java version.<br>
**4.** Create the `main/java` directory in the src directory. This is where you will be creating your 
Java classes for your assignment. Right click `src` and go to New > Directory and select `main/java`.<br>

### Problem 1

1. In the `main/java` directory, create a class named `Makes10`. 
2. Create a `public static` method named `numberInfo`. This method should take two integer parameters (you
   choose the variable names!) and return a `String`. 
3. The method should determine whether the two integers sum up to 10 or if one of them is 10.
    * If the parameters sum up to 10, but neither number is 10, return the String `"Sum is 10. Neither number is 10."`
    * If the parameters sum up to 10 and one or both of the numbers is 10, return the String `"Sum is 10. One or both
    numbers are 10."`
    * If the parameters do not sum up to 10, but one or both of the numbers is 10, return the String `"Sum is not 10. 
    One or both numbers are 10."`
    * If the parameters do not sum up to 10 and neither of the numbers is 10, return the String `"Sum is not 10.
      Neither number is 10."`
4. Create the `main` method. In the `main` method, do the following:
    * Call the `numberInfo` method and pass in -10 and 20 for the parameters. Assign the returned value to a
      String variable. Print out the String variable. The output should be: `"Sum is 10. Neither number is 10."`
      Is your output correct?
    * Call the `numberInfo` method and pass in 10 and 33 for the parameters. Assign the returned value to a
      String variable. Print out the String variable. The output should be: `"Sum is not 10. One or both
      numbers are 10."` Is your output correct?
    * Call the `numberInfo` method and pass in 10 and 0 for the parameters. Assign the returned value to a
      String variable. Print out the String variable. The output should be: `"Sum is 10.
      One or both numbers are 10."` Is your output correct?
    * Call the `numberInfo` method and pass in 3 and 12 for the parameters. Assign the returned value to a
      String variable. Print out the String variable. The output should be: `"Sum is not 10.
      Neither number is 10."` Is your output correct?
    * Call the `numberInfo` method and pass in 10 and 10 for the parameters. Assign the returned value to a
      String variable. Print out the String variable. The output should be: `"Sum is not 10. One or both
      numbers are 10."` Is your output correct?
5. Uncomment the tests in the `Makes10Test` class in the `test/java` folder. Run the tests.
6. Run the `checkstyleMain` task. Run the `pmdMain` task. Remember that error reports are in the `build/reports`
   folder.


### Problem 2

1. In the `main/java` directory, create a class named `NumberSpacing`. 
2. Create a `public static` method named `evenlySpaced`. This method should take three integer parameters (you
   choose the variable names!) and return a `boolean`.
3. The three integer parameters are unique values. One of the integers is the smallest, one integer is largest, 
   and one is in between the other two. 
    * Return `true` if the three values are evenly spaced (the difference between the smallest and largest 
      is the same as the difference between the middle and largest).
    * Otherwise, return false.
4. Create the `main` method. In the `main` method, do the following:
    * Call the `evenlySpaced` method and pass in 2, 4, and 6 for the parameters (in that order). Assign the 
      returned value to a boolean variable. Print out the boolean variable. This output should be true. Is 
      your output correct?
    * Call the `evenlySpaced` method and pass in 4, 6, and 2 for the parameters (in that order). Assign the
      returned value to a boolean variable. Print out the boolean variable. This output should be true. Is
      your output correct?
    * Call the `evenlySpaced` method and pass in 9, 1, and 3 for the parameters (in that order). Assign the
     returned value to a boolean variable. Print out the boolean variable. This output should be false. Is
     your output correct?
5. Uncomment the tests in the `NumberSpacingTest` class in the `test/java` folder. Run the tests.
6. Run the `checkstyleMain` task. Run the `pmdMain` task. Remember that error reports are in the `build/reports`
   folder.