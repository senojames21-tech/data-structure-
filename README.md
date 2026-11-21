mport java.util.HashMap;

public class Main {
    public static void main(String[] args) {

        // Create a HashMap
        // Integer = Student ID (Key)
        // String = Student Name (Value)
        HashMap<Integer, String> students =
                new HashMap<Integer, String>();

        // ADD ELEMENTS
        students.put(1001, "Juan Dela Cruz");
        students.put(1002, "Maria Santos");
        students.put(1003, "Pedro Garcia");
        students.put(1004, "Ana Reyes");
        students.put(1004, "Ana Reyes"); // Duplicate Key
        students.put(1005, "John Lim");

        // DISPLAY ALL STUDENTS
        System.out.println("All Students:");
        System.out.println(students);

        // DISPLAY A SPECIFIC STUDENT
        System.out.println("\nStudent with ID 1002:");
        System.out.println(students.get(1002));

        // UPDATE A STUDENT'S NAME
        students.put(1003, "Pedro Ramirez");

        System.out.println("\nAfter Updating Student ID 1003:");
        System.out.println(students);

        // REMOVE A STUDENT
        students.remove(1001);

        System.out.println("\nAfter Removing Student ID 1001:");
        System.out.println(students);

        // CHECK IF A KEY EXISTS
        System.out.println("\nIs Student ID 1005 existing?");
        System.out.println(students.containsKey(1005));

        // DISPLAY NUMBER OF STUDENTS
        System.out.println("\nTotal Students:");
        System.out.println(students.size());

        // CLEAR ALL ELEMENTS
        students.clear();

        // DISPLAY ALL ELEMENTS
        System.out.println("\nAfter Clearing All Students:");
        System.out.println(students);
    }
}
