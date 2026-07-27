import java.util.Scanner;

public class Day3Fibonacci {

	public static int ReturnBack(int SequenceIRB) {
		if (SequenceIRB <= 2) {
			return 1;
		}
		
		return ReturnBack(SequenceIRB - 1) + ReturnBack(SequenceIRB - 2);	
	}

	public static int Repeat(int SequenceIR) {
		
		if (SequenceIR <= 2) {
			return 1;
		}
		
		int First = 0;
		int Second = 1;
		int Result= 0;
		
		for(int i = 2; i <= SequenceIR; i++) {
			Result = First + Second;
			First = Second;
			Second = Result;
		}
		return Result;
	}

	public static void main(String[] args) {
		Scanner Sc = new Scanner(System.in, "MS949");
		
		System.out.println("몇 번째 수열까지 구하시겠어요?");
		int Sequence = Sc.nextInt();

		System.out.println("다음중 어떤 방식으로 수열을 구하시겠어요?");
		System.out.println("[1]: 재귀 함수");
		System.out.println("[2]: 반복문 함수");
		int Construction = Sc.nextInt();

		if (Construction == 1) {
			int SequenceResult = ReturnBack(Sequence);
			System.out.println("[" + Construction + "]번 방식으로 계산해 구한 " + "피보차니 수열의 " + Sequence + "번은" + " [" + SequenceResult + "]입니다.");
		} else if (Construction == 2) {
			int SequenceResult = Repeat(Sequence);
			System.out.println("[" + Construction + "]번 방식으로 계산해 구한 " + "피보차니 수열의  " + Sequence + "번은" + " [" + SequenceResult + "]입니다.");
		}
	
	}
}
		
