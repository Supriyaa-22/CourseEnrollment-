# CourseEnrollment-

import java.util.ArrayList;
import java.util.Scanner;

public class CourseEnrollmentSearch {
    public static void main(String[] args) {
        ArrayList<String> students = new ArrayList<>();

        students.add("Riya");
        students.add("Neha");
        students.add("Reena");
        students.add("Charlie");
        students.add("David");

        Scanner sc = new Scanner(System.in);
        System.out.print("Enter student name to search: ");
        String searchName = sc.nextLine();

        if (students.contains(searchName)) {
            System.out.println("" + searchName + " is enrolled in the course.");
        } else {
            System.out.println("" + searchName + " is NOT enrolled in the course.");
        }
        sc.close();
    }
}
