import java.util.*;

public class TaskManager {
    public static List<String> removeDuplicates(List<String> tasks) {
        Set<String> uniqueTasks = new LinkedHashSet<>(tasks);
        return new ArrayList<>(uniqueTasks);
    }

    public static void main(String[] args) {
        List<String> tasks = Arrays.asList("Завдання 1", "Завдання 2", "Завдання 1", "Завдання 3", "Завдання 2");
        System.out.println("Оригінальний список: " + tasks);

        List<String> result = removeDuplicates(tasks);
        System.out.println("Список без дублікатів: " + result);
    }
}
 
