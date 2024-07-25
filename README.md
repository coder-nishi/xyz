import java.util.ArrayList;

public class ArrayListExample {
    public static void main(String[] args) {
        // Creating an ArrayList of Strings
        ArrayList<String> fruits = new ArrayList<>();

       
        fruits.add("Apple");
        fruits.add("Banana");
        fruits.add("Orange");
        fruits.add("Mango");

       
        System.out.println("ArrayList: " + fruits);

        
        System.out.println("First fruit: " + fruits.get(0));
        System.out.println("Third fruit: " + fruits.get(2));

       
        String searchFruit = "Banana";
        if (fruits.contains(searchFruit)) {
            System.out.println(searchFruit + " is present in the ArrayList.");
        } else {
            System.out.println(searchFruit + " is not present in the ArrayList.");
        }

      
        fruits.remove("Orange");
        System.out.println("After removing 'Orange': " + fruits);

        
        System.out.println("Iterating over ArrayList:");
        for (String fruit : fruits) {
            System.out.println(fruit);
        }

       
        System.out.println("Size of ArrayList: " + fruits.size());

      
        fruits.clear();
        System.out.println("After clearing ArrayList: " + fruits);
    }
}

