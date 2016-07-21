# ArrayCheckSameIndex
import java.util.Arrays;
import java.util.Scanner;

public class ArrayCheck {

	public static void main(String[] args) {
		Scanner qq = new Scanner(System.in);
		System.out.println("enter size of array");
		int nn = qq.nextInt();
		int count[] = new int[nn];
		System.out.println("enter array element");
		for (int i = 0; i < nn; i++) {
			count[i] = qq.nextInt();
		}
		Arrays.sort(count);
		int ind = 0;
		for (int j = 0; j < count.length; j++) {
			if (count[j] == j) {
				ind = 1;
				System.out.println("element " + count[j] + " is same as index");
			}
		}
		if (ind == 0) {
			System.out.println("no element is same as index");
		}

	}

}
