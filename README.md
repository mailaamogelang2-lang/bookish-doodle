# bookish-doodle

import java.util.ArrayList;
import java.util.Scanner;

public class Checklist {

    public static void main(String[] args) {

        ArrayList<String> tasks = new ArrayList<>();
        Scanner input = new Scanner(System.in);

        while (true) {

            System.out.println("Checklist Menu");
            System.out.println("1. Add Task");
            System.out.println("2. View Tasks");
            System.out.println("3. Exit");
            System.out.println("Choose: ");

            int choice = input.nextInt();
            input.nextLine(); 

            if (choice == 1) {

                System.out.print("Enter a task: ");
                String task = input.nextLine();
                tasks.add(task);
                System.out.println("Task added");

            } else if (choice == 2) {

                System.out.println("Your Tasks is:");
              
                    System.out.println("No tasks yet.");
                
            } 

            } else {

                System.out.println("Invalid choice.");
            }
        }

        input.close();
    }
}
