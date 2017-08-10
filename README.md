
# Java-Strings:We needs to change the content for the following methods.

1.byte getBytes():

Example:
```
import java.io.UnsupportedEncodingException;

public class Test {

	public static void main(String args[]) {
		String Str1 = new String("Welcome to Revature.com");

		try {
			byte[] Str2 = Str1.getBytes();
			System.out.println("Returned  Value " + Str2);

			Str2 = Str1.getBytes("UTF-8");
			System.out.println("Returned  Value " + Str2);

			Str2 = Str1.getBytes("ISO-8859-1");
			System.out.println("Returned  Value " + Str2);
		} catch (UnsupportedEncodingException e) {
			System.out.println("Unsupported character set");
		}
	}
}
```

This produces the following result:

Returned  Value [B@659e0bfd
Returned  Value [B@2a139a55
Returned  Value [B@15db9742

2.byte[] getBytes(String charsetName):

Example:
```
import java.io.*;

public class Test {

	public static void main(String args[]) {
		String Str1 = new String("Welcome to Revature.com");

		try {
			byte[] Str2 = Str1.getBytes();
			System.out.println("Returned  Value " + Str2);

			Str2 = Str1.getBytes("UTF-8");
			System.out.println("Returned  Value " + Str2);

			Str2 = Str1.getBytes("ISO-8859-1");
			System.out.println("Returned  Value " + Str2);
		} catch (UnsupportedEncodingException e) {
			System.out.println("Unsupported character set");
		}
	}
}
```
This produces the following result:

Returned  Value [B@659e0bfd
Returned  Value [B@2a139a55
Returned  Value [B@15db9742



