
# Java-Strings:
              We needs to change the content for the following method examples.
	      
1.byte getBytes():

Example:

```java
import java.io.UnsupportedEncodingException;

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
import java.io.UnsupportedEncodingException;

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

Note:The above two overloaded methods byte[] getBytes(String charsetName),byte getBytes() are differing with the tutorialspoint content example.
Please refer this url:https://www.tutorialspoint.com/java/java_string_getbytes_charsetname.htm. If you are observing,in these two overloaded method examples we are storing the results in byte[],but in tutorialspoint they are storing the results in String.


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

10.int lastIndexOf(int ch, int fromIndex):

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

11.int lastIndexOf(String str):

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

12.int lastIndexOf(String str, int fromIndex):

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

13.int length():

Example:

```java
public class Test{
	   public static void main(String args[]){
	      String str1 = new String("Welcome to Revature.com");
	      String str2 = new String("Revature" );

	      System.out.print("String Length :" );
	      System.out.println(str1.length());

	      System.out.print("String Length :" );
	      System.out.println(str2.length());
	   }
	}
	
This produces the following result:

String Length :23
String Length :8
```
	
14.boolean matches(String regex):

Example:

```java
public class Test {
	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");

		System.out.print("Return Value :");
		System.out.println(str.matches("(.*)Revature(.*)"));

		System.out.print("Return Value :");
		System.out.println(str.matches("Revature"));

		System.out.print("Return Value :");
		System.out.println(str.matches("Welcome(.*)"));
	}
}

This produces the following result:

Return Value :true
Return Value :false
Return Value :true
```

15.boolean regionMatches(boolean ignoreCase, int toffset, String other, int ooffset, int len):

Example:

```java
public class Test {
	public static void main(String args[]) {
		String str1 = new String("Welcome to Revature.com");
		String str2 = new String("Revature");
		String str3 = new String("REVATURE");

		System.out.print("Return Value :");
		System.out.println(str1.regionMatches(11, str2, 0, 8));

		System.out.print("Return Value :");
		System.out.println(str1.regionMatches(11, str3, 0, 8));

		System.out.print("Return Value :");
		System.out.println(str1.regionMatches(true, 11, str3, 0, 8));
	}
}


This produces the following result:

Return Value :true
Return Value :false
Return Value :true
```

16.boolean regionMatches(int toffset, String other, int ooffset, int len):

Example:

```java
public class Test {
	public static void main(String args[]) {
		String str1 = new String("Welcome to Revature.com");
		String str2 = new String("Revature");
		String str3 = new String("REVATURE");

		System.out.print("Return Value :");
		System.out.println(str1.regionMatches(11, str2, 0, 8));

		System.out.print("Return Value :");
		System.out.println(str1.regionMatches(11, str3, 0, 8));

		System.out.print("Return Value :");
		System.out.println(str1.regionMatches(true, 11, str3, 0, 8));
	}
}


This produces the following result:

Return Value :true
Return Value :false
Return Value :true
```

17.String replace(char oldChar, char newChar):

Example:

```java
public class Test {
	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");

		System.out.print("Return Value :");
		System.out.println(str.replace('o', 'T'));

		System.out.print("Return Value :");
		System.out.println(str.replace('l', 'D'));
	}
}

This produces the following result:

Return Value :WelcTme tT Revature.cTm
Return Value :WeDcome to Revature.com
```

18.String replaceAll(String regex, String replacement):

Example:

```java
public class Test {
	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");

		System.out.print("Return Value :");
		System.out.println(str.replaceAll("(.*)Revature(.*)", "AMROOD"));
	}
}

This produces the following result:

Return Value :AMROOD
```

19.String replaceFirst(String regex, String replacement):

Example:

```java
public class Test {
	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");

		System.out.print("Return Value :");
		System.out.println(str.replaceFirst("(.*)Revature(.*)", "AMROOD"));

		System.out.print("Return Value :");
		System.out.println(str.replaceFirst("Revature", "AMROOD"));
	}
}

This produces the following result:

Return Value :AMROOD
Return Value :Welcome to AMROOD.com
```

20.boolean startsWith(String prefix):

Example:

```java
public class Test {
	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");

		System.out.print("Return Value :");
		System.out.println(str.startsWith("Welcome"));

		System.out.print("Return Value :");
		System.out.println(str.startsWith("Revature"));

		System.out.print("Return Value :");
		System.out.println(str.startsWith("Revature", 11));
	}
}

This produces the following result:

Return Value :true
Return Value :false
Return Value :true
```

21.boolean startsWith(String prefix, int toffset):

Example:

```java
public class Test {
	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");

		System.out.print("Return Value :");
		System.out.println(str.startsWith("Welcome"));

		System.out.print("Return Value :");
		System.out.println(str.startsWith("Revature"));

		System.out.print("Return Value :");
		System.out.println(str.startsWith("Revature", 11));
	}
}

This produces the following result:

Return Value :true
Return Value :false
Return Value :true
```

22.CharSequence subSequence(int beginIndex, int endIndex):

Example:

```java
public class Test {
	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");

		System.out.print("Return Value :");
		System.out.println(str.subSequence(0, 10));

		System.out.print("Return Value :");
		System.out.println(str.subSequence(10, 15));
	}
}

This produces the following result:

Return Value :Welcome to
Return Value : Reva
```

23.String substring(int beginIndex):

Example:

```java
public class Test {
	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");

		System.out.print("Return Value :");
		System.out.println(str.substring(10));

		System.out.print("Return Value :");
		System.out.println(str.substring(10, 15));
	}
}

This produces the following result:

Return Value : Revature.com
Return Value : Reva
```

24.String substring(int beginIndex, int endIndex):

Example:

```java
public class Test {
	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");

		System.out.print("Return Value :");
		System.out.println(str.substring(10));

		System.out.print("Return Value :");
		System.out.println(str.substring(10, 15));
	}
}

This produces the following result:

Return Value : Revature.com
Return Value : Reva
```

25.String toUpperCase():

Example:

```java
public class Test {
	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");

		System.out.print("Return Value :");
		System.out.println(str.toUpperCase());
	}
}

This produces the following result:

Return Value :WELCOME TO REVATURE.COM
```

26.String toUpperCase(Locale locale):

Example:

```java
public class Test {
	public static void main(String args[]) {
		String str = new String("Welcome to Revature.com");

		System.out.print("Return Value :");
		System.out.println(str.toUpperCase());
	}
}

This produces the following result:

Return Value :WELCOME TO REVATURE.COM
```

Note:In the above code snippets,if you are observing the overloaded methods are having the same code.Instead of writing seperately,we can reuse the same code or we can pass different input data.




