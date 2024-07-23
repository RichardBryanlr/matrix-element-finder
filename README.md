package application;

import java.util.Scanner;

public class Program {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);

		System.out.print("Enter a number of lines X: ");
		int lineX = sc.nextInt();

		System.out.print("Enter a number of columns Y: ");
		int lineY = sc.nextInt();
		System.out.println();

		int[][] matrix = new int[lineX][lineY];

		for (int i = 0; i < lineX; i++) {
			for (int j = 0; j < lineY; j++) {
				matrix[i][j] = sc.nextInt();
			}
			System.out.println();
		}

		System.out.print("Enter a number to find in matrix: ");
		int findNumber = sc.nextInt();
		System.out.println();

		for(int i = 0; i < lineX; i++) {
			for(int j = 0; j < lineY; j++) {
				if(matrix[i][j] == findNumber) {
					System.out.print("[" + matrix[i][j] + "]	");
				} else {
					System.out.print(" " + matrix[i][j] + " 	");
				}
				
			}
			System.out.println("\n");
		}

		for (int i = 0; i < lineX; i++) {
			for (int j = 0; j < lineY; j++) {
				if (matrix[i][j] == findNumber) {
					System.out.println("Position: " + "X: " + i + ", Y: " + j);
					
					if(i - 1 >= 0) {
						System.out.println("number up:	" + matrix[i-1][j]);
					} else {
						System.out.println("number up:	none");
					}
					
					if(j - 1 >= 0) {
						System.out.println("number left:	" + matrix[i][j-1]);
					} else {
						System.out.println("number left:	none");
					}
					
					if(j + 1 < lineY) {
						System.out.println("number right:	" + matrix[i][j+1]);
					} else {
						System.out.println("number right:	none");
					}
					
					if(i + 1 < lineX) {
						System.out.println("number bottom:	" + matrix[i+1][j]);
					} else {
						System.out.println("number bottom:	none");
					}

				}
			}
			System.out.println();
		}

		sc.close();
	}
}
