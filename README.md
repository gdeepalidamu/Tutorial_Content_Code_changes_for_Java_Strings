
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
		String Str1 = new String("Welcome to Revature.com");
		char[] Str2 = new char[7];

		try {
			Str1.getChars(2, 9, Str2, 0);
			System.out.print("Copied Value = ");
			System.out.println(Str2);

		} catch (Exception ex) {
			System.out.println("Raised exception...");
		}
	}
}

This produces the following result:

Copied Value = lcome t
```
