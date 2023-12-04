Part 1 – Debugging Scenario
Design a debugging scenario, and write your report as a conversation on EdStem. It should have:

1. The original post from a student with a screenshot showing a symptom and a description of a guess at the bug/some sense of what the failure-inducing input is. (Don’t actually make the post! Just write the content that would go in such a post)

Student "Hi Afraz, I hope you're having a good day so far. I'm trying to get my code to work, my student submission file is not working and I have tried debugging it, and don't know what to do.  The screenshot of the failed tests is shown below, I'm thinking it's giving an out of bounds error because there is a missing curly brace so even though the index is in the same area under the if statement, the if statement isn't registering it. Sincerely, Akhil." 


![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/7edb827b-0d61-49d2-b892-f78c4a293a13)

Code with bug:

```
import java.util.ArrayList;
import java.util.List;

interface StringChecker { boolean checkString(String s); }

class ListExamples {

  // Returns a new list that has all the elements of the input list for which
  // the StringChecker returns true, and not the elements that return false, in
  // the same order they appeared in the input list;
  static List<String> filter(List<String> list, StringChecker sc) {
    List<String> result = new ArrayList<>();
    for(String s: list) {
      if(sc.checkString(s)) {
        result.add(s);
      }
    }
    return result;
  }


  // Takes two sorted list of strings (so "a" appears before "b" and so on),
  // and return a new list that has all the strings in both list in sorted order.
  static List<String> merge(List<String> list1, List<String> list2) {
    List<String> result = new ArrayList<>();
    int index1 = 0, index2 = 0;
    while(index1 < list1.size() && index2 < list2.size()) {
      if(list1.get(index1).compareTo(list2.get(index2)) < 0) {
        index1 += 1;
        result.add(list1.get(index1));

      }
      else {
        result.add(list2.get(index2));
        index2 += 1;
      }
    }
    while(index1 < list1.size()) {
      result.add(list1.get(index1));
      index1 += 1;
    }
    while(index2 < list2.size()) {
      result.add(list2.get(index2));
      index2 += 1;
    }
    return result;
  }


}
```

2. A response from a TA asking a leading question or suggesting a command to try (To be clear, you are mimicking a TA here.)

Afraz TA - Hey Akhil, Run a print statement that prints list1 and result after each iteration of the first while loop and see how it changes over time.

3. Another screenshot/terminal output showing what information the student got from trying that, and a clear description of what the bug is.

Student - Oh, let me try that - I will look through the if statement and see if anything is off.


The bug is that the index1 += 1 is happening before the result.add(list1.get(index1)); 

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/9f733639-d5bf-4f8c-8112-8c7dcd5e6b90)


Student - I see that result prints out b and c but not a, so I think the index1 value is skipping the first element and doesn't print out a from list1.

4. At the end, all the information needed about the setup including:
The file & directory structure needed
The contents of each file before fixing the bug
The full command line (or lines) you ran to trigger the bug
A description of what to edit to fix the bug


File and directroy structure needed: You need to have ListExamples.java and test.sh in the same directory, along with the ListExamplesTests.java to run the tests on ListExamples.java, since the test.sh uses the ListExamplesTests.java file to run evaluations on the ListExamples.java class. 

Content of files before fixing bug:

`test.sh`

`javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java
java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests`

`ListExamples.java`

```
import java.util.ArrayList;
import java.util.List;

interface StringChecker { boolean checkString(String s); }

class ListExamples {

  // Returns a new list that has all the elements of the input list for which
  // the StringChecker returns true, and not the elements that return false, in
  // the same order they appeared in the input list;
  static List<String> filter(List<String> list, StringChecker sc) {
    List<String> result = new ArrayList<>();
    for(String s: list) {
      if(sc.checkString(s)) {
        result.add(s);
      }
    }
    return result;
  }


  // Takes two sorted list of strings (so "a" appears before "b" and so on),
  // and return a new list that has all the strings in both list in sorted order.
  static List<String> merge(List<String> list1, List<String> list2) {
    List<String> result = new ArrayList<>();
    int index1 = 0, index2 = 0;
    while(index1 < list1.size() && index2 < list2.size()) {
      if(list1.get(index1).compareTo(list2.get(index2)) < 0) {
        index1 += 1;
        result.add(list1.get(index1));

      }
      else {
        result.add(list2.get(index2));
        index2 += 1;
      }
    }
    while(index1 < list1.size()) {
      result.add(list1.get(index1));
      index1 += 1;
    }
    while(index2 < list2.size()) {
      result.add(list2.get(index2));
      index2 += 1;
    }
    return result;
  }


}
```

![image](https://github.com/TTVTechTaro/cse15l-lab-reports/assets/46509287/7f8a0e58-d1a9-4c5d-9624-705259f58f6a)

Correct code:

```
// Takes two sorted list of strings (so "a" appears before "b" and so on),
  // and return a new list that has all the strings in both list in sorted order.
  static List<String> merge(List<String> list1, List<String> list2) {
import java.util.ArrayList;
import java.util.List; 
interface StringChecker { boolean checkString(String s); }

class ListExamples { 

  // Returns a new list that has all the elements of the input list for which
  // the StringChecker returns true, and not the elements that return false, in
  // the same order they appeared in the input list; 
  import java.util.ArrayList;
import java.util.List;

interface StringChecker { boolean checkString(String s); }

class ListExamples {

  // Returns a new list that has all the elements of the input list for which
  // the StringChecker returns true, and not the elements that return false, in
  // the same order they appeared in the input list;
  static List<String> filter(List<String> list, StringChecker sc) {
    List<String> result = new ArrayList<>();
    for(String s: list) {
      if(sc.checkString(s)) {
        result.add(s);
      }
    }
    return result;
  }


  // Takes two sorted list of strings (so "a" appears before "b" and so on),
  // and return a new list that has all the strings in both list in sorted order.
  static List<String> merge(List<String> list1, List<String> list2) {
    List<String> result = new ArrayList<>();
    int index1 = 0, index2 = 0;
    while(index1 < list1.size() && index2 < list2.size()) {
      if(list1.get(index1).compareTo(list2.get(index2)) < 0) {
        result.add(list1.get(index1));
        index1 += 1;
      }
      else {
        result.add(list2.get(index2));
        index2 += 1;
      }
    }
    while(index1 > list1.size()) {
      result.add(list1.get(index1));
      index1 += 1;
    }
    while(index2 < list2.size()) {
      result.add(list2.get(index2));
      index2 += 1;
    }
    return result;
  }


}
```

To fix the bug you need to move the index1 += 1 and move it to be after the result.add(list1.get(index1), since that results in the first value being skipped in list1 and not being properly merged in the Result arraylist.

Part 2 – Reflection

I learned about `grep` and how you can use it to search for the lines that contain a specific string in a file, and how you can use that command even furhter in different ways like -i to instead return all the lines in a file that do NOT contain the string. In addition, there are other types of commands to navigate file structure like `ls` to list out things in a directory, `cd` to switch to different directories, and `cat` to concatenate and print out files, ways to edit files via terminal with vim, methods to perform git commands via the terminal, and more. All in all, I've found very robust and quick ways to do many tasks on terminal without needing to open up a single website, so much can be done just by terminal, as we showed in Skill Demo 4, doing an entire skill demo via terminal.
