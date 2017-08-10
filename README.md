
# Java-Strings:We needs to change the content for the following methods.

1.byte getBytes():

Example:

```java
import java.io.*;

public class Test {

	public static void main(String args[]) {
		String str1 = new String("Welcome to Revature.com");

		try {
			byte[] str2 = str1.getBytes();
			System.out.println("Returned  Value " + str2);

			str2 = str1.getBytes("UTF-8");
			System.out.println("Returned  Value " + str2);

			str2 = str1.getBytes("ISO-8859-1");
			System.out.println("Returned  Value " + str2);
		} catch (UnsupportedEncodingException e) {
			System.out.println("Unsupported character set");
		}
	}
}

This produces the following result:

Returned  Value [B@659e0bfd
Returned  Value [B@2a139a55
Returned  Value [B@15db9742
```
2.byte[] getBytes(String charsetName):

Example:

```java
import java.io.*;

public class Test {

	public static void main(String args[]) {
		String str1 = new String("Welcome to Revature.com");

		try {
			byte[] str2 = str1.getBytes();
			System.out.println("Returned  Value " + str2);

			str2 = str1.getBytes("UTF-8");
			System.out.println("Returned  Value " + str2);

			str2 = str1.getBytes("ISO-8859-1");
			System.out.println("Returned  Value " + str2);
		} catch (UnsupportedEncodingException e) {
			System.out.println("Unsupported character set");
		}
	}
}

This produces the following result:

Returned  Value [B@659e0bfd
Returned  Value [B@2a139a55
Returned  Value [B@15db9742
```

3.void getChars(int srcBegin, int srcEnd, char[] dst, int dstBegin):

Example:

```java
public class Test {
	public static void main(String args[]) {
		String str1 = new String("Welcome to Revature.com");
		char[] str2 = new char[7];

		try {
			str1.getChars(2, 9, str2, 0);
			System.out.print("Copied Value = ");
			System.out.println(str2);

		} catch (Exception ex) {
			System.out.println("Raised exception...");
		}
	}
}

This produces the following result:

Copied Value = lcome t
```

4.int hashCode():

Example:

```java
public class Test{
   public static void main(String args[]){
      String str = new String("Welcome to Revature.com");
      System.out.println("Hashcode for str :" + str.hashCode() );
   }
}

This produces the following result:

Hashcode for str :-1924542484
```

5.int indexOf(int ch):

Example:

```java
public class Test {

	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");
		String subStr1 = new String("Revature");
		String subStr2 = new String("Sevature");

		System.out.print("Found Index :");
		System.out.println(str.indexOf('o'));
		System.out.print("Found Index :");
		System.out.println(str.indexOf('o', 5));
		System.out.print("Found Index :");
		System.out.println(str.indexOf(subStr1));
		System.out.print("Found Index :");
		System.out.println(str.indexOf(subStr1, 15));
		System.out.print("Found Index :");
		System.out.println(str.indexOf(subStr2));
	}
}

This produces the following result:

Found Index :4
Found Index :9
Found Index :11
Found Index :-1
Found Index :-1
```

6.int indexOf(int ch, int fromIndex):

Example:

```java
public class Test {

	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");
		String subStr1 = new String("Revature");
		String subStr2 = new String("Sevature");

		System.out.print("Found Index :");
		System.out.println(str.indexOf('o'));
		System.out.print("Found Index :");
		System.out.println(str.indexOf('o', 5));
		System.out.print("Found Index :");
		System.out.println(str.indexOf(subStr1));
		System.out.print("Found Index :");
		System.out.println(str.indexOf(subStr1, 15));
		System.out.print("Found Index :");
		System.out.println(str.indexOf(subStr2));
	}
}

This produces the following result:

Found Index :4
Found Index :9
Found Index :11
Found Index :-1
Found Index :-1
```

7.int indexOf(String str):

Example:

```java
public class Test {

	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");
		String subStr1 = new String("Revature");
		String subStr2 = new String("Sevature");

		System.out.print("Found Index :");
		System.out.println(str.indexOf('o'));
		System.out.print("Found Index :");
		System.out.println(str.indexOf('o', 5));
		System.out.print("Found Index :");
		System.out.println(str.indexOf(subStr1));
		System.out.print("Found Index :");
		System.out.println(str.indexOf(subStr1, 15));
		System.out.print("Found Index :");
		System.out.println(str.indexOf(subStr2));
	}
}

This produces the following result:

Found Index :4
Found Index :9
Found Index :11
Found Index :-1
Found Index :-1
```

8.int indexOf(String str, int fromIndex):

Example:

```java
public class Test {

	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");
		String subStr1 = new String("Revature");
		String subStr2 = new String("Sevature");

		System.out.print("Found Index :");
		System.out.println(str.indexOf('o'));
		System.out.print("Found Index :");
		System.out.println(str.indexOf('o', 5));
		System.out.print("Found Index :");
		System.out.println(str.indexOf(subStr1));
		System.out.print("Found Index :");
		System.out.println(str.indexOf(subStr1, 15));
		System.out.print("Found Index :");
		System.out.println(str.indexOf(subStr2));
	}
}

This produces the following result:

Found Index :4
Found Index :9
Found Index :11
Found Index :-1
Found Index :-1
```

9.int lastIndexOf(int ch):

Example:

```java
public class Test {

	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");
		String subStr1 = new String("Revature");
		String subStr2 = new String("Sevature");

		System.out.print("Found Last Index :");
		System.out.println(str.lastIndexOf('o'));
		System.out.print("Found Last Index :");
		System.out.println(str.lastIndexOf('o', 5));
		System.out.print("Found Last Index :");
		System.out.println(str.lastIndexOf(subStr1));
		System.out.print("Found Last Index :");
		System.out.println(str.lastIndexOf(subStr1, 15));
		System.out.print("Found Last Index :");
		System.out.println(str.lastIndexOf(subStr2));
	}
}

This produces the following result:

Found Last Index :21
Found Last Index :4
Found Last Index :11
Found Last Index :11
Found Last Index :-1
```


