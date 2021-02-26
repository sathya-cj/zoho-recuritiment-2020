package com.interview.Zoho;

public class zohoprgm1 {

	public static void getHalfPyramid(String str, int len) {
		int mid = 0;
		for (int i = 1; i <= len; i++) {
			if ((len % 2) == 0)
				mid = (len / 2) - 1;
			else
				mid = (len / 2);
				for (int k = 0; k < len - i; k++) {
					System.out.print(" ");
				}
				for (int p = 0; p < i; p++) {
					System.out.print(str.charAt(mid));
					if (mid != len-1)
						mid++;
					else
						mid = 0;
				}

		
			System.out.println();
		}
	}

	public static void main(String[] args) {
		String str = "WELCOME";
		int len = str.length();
		getHalfPyramid(str, len);
	}
}
