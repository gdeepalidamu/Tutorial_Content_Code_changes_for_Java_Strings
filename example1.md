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
