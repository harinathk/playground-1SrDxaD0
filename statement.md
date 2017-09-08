# Convert String to Char Array

Use String.toCharArray() to convert a String into a char array

```java runnable
// { autofold
public class Main {

public static void main(String[] args) {
// }

 String techioStr = "TechIO Playground";
 char[] techioCharArray = techioStr.toCharArray();
 for (char techioChar : techioCharArray) {
    System.out.println(techioChar);
 }

//{ autofold
}

}
//}
```
# Convert String to Char Array Using Java 8
Use .chars() to get the IntStream, and convert it to Stream Char using .mapToObj

```java runnable
// { autofold
public class Main {

public static void main(String[] args) {
// }
 String techioStr = "TechIO Playground";
 techioStr.chars() //IntStream
         .mapToObj(x -> (char) x)//Stream<Character>
        .forEach(System.out::println);

//{ autofold
}

}
//}
```
