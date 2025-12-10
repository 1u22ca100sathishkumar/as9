# as9
1. Program to print elements from a List using a normal for loop
import java.util.*;

public class ListExample {
    public static void main(String[] args) {
        List<String> list = Arrays.asList("Apple", "Banana", "Cherry");

        for (int i = 0; i < list.size(); i++) {
            System.out.println(list.get(i));
        }
    }
}

2. Program to store elements in a Set and print them in sorted order
import java.util.*;

public class SetExample {
    public static void main(String[] args) {
        Set<Integer> numbers = new HashSet<>();
        numbers.add(30);
        numbers.add(10);
        numbers.add(20);

        // Convert to a TreeSet for sorting
        Set<Integer> sortedSet = new TreeSet<>(numbers);

        System.out.println("Sorted Set Elements:");
        for (int num : sortedSet) {
            System.out.println(num);
        }
    }
}

3. Program to store elements in a Map<String, String> and print them
import java.util.*;

public class MapExample {
    public static void main(String[] args) {
        Map<String, String> map = new HashMap<>();

        map.put("101", "Alice");
        map.put("102", "Bob");
        map.put("103", "Charlie");

        System.out.println("Map Elements:");
        for (Map.Entry<String, String> entry : map.entrySet()) {
            System.out.println(entry.getKey() + " : " + entry.getValue());
        }
    }
}
