//SortLetters.java
//Program that generates 30 random characters and prints them in certain orders
//By Ruhul Shah

import java.util.Comparator;
import java.util.ArrayList;
import java.util.List;
import java.util.stream.Collectors;

public class SortLetters {
	 public static void main(String args[]) {
		 List<Character> listRandomChars = new ArrayList<>();
		 //generate 30 random chars and add to list
		 for (int i=0; i<30; i++) {
			 int num = (int) (26* Math.random());
			 char letter = (char) (num + 'a');
			 listRandomChars.add(letter);
		 }//end for loop
		 
		 //display ascending list
		 List<Character> listAscSortedChars = listRandomChars.stream()
				 										.sorted()
				 										.collect(Collectors.toList());
		 System.out.println("Ascending Order: " + listAscSortedChars);
		 
		 //display descending list
		 List<Character> listDscSortedChars = listRandomChars.stream()
				 										.sorted(Comparator.reverseOrder())
				 										.collect(Collectors.toList());
		System.out.println("Descending Order: " + listDscSortedChars);		
		 
		//display ascending list without duplicates
		 List<Character> listAscSortedUniqueChars = listRandomChars.stream()
														.sorted()
														.distinct()
														.collect(Collectors.toList());
		 System.out.println("Unique Ascending Order: " + listAscSortedUniqueChars);
		 
	 }//end main method
}
