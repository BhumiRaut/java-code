# java-code
pavkage p;
public class A1{

    public static <T> void checkElements(T[] array, T e1, T e2) {
        int index1 = -1;
        int index2 = -1;

        for (int i = 0; i < array.length; i++) {
            if (array[i].equals(e1)) {
                index1 = i;
            }
            if (array[i].equals(e2)) {
                index2 = i;
            }
        }

        if (index1 != -1 && index2 != -1) {
            System.out.println(e1 + " found at index: " + index1);
            System.out.println(e2 + " found at index: " + index2);
        } else {
            System.out.println("One or both elements not found.");
        }
    }

    public static void main(String[] args) {
        Integer[] numbers = {10, 20, 30, 40, 50};

        checkElements(numbers, 20, 50);  
        checkElements(numbers, 20, 100);  
    }
}
