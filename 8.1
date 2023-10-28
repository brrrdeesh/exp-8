import java.util.Scanner;

class NumberInputThread extends Thread {
    private int[] numbers;
    
    public void run() {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of elements: ");
        int n = scanner.nextInt();
        numbers = new int[n];
        System.out.println("Enter " + n + " numbers:");
        
        for (int i = 0; i < n; i++) {
            numbers[i] = scanner.nextInt();
        }
        
        scanner.close();
    }
    
    public int[] getNumbers() {
        return numbers;
    }
}

class DivisibleByFiveThread extends Thread {
    private int[] numbers;
    
    public DivisibleByFiveThread(int[] numbers) {
        this.numbers = numbers;
    }
    
    public void run() {
        System.out.println("Numbers divisible by five:");
        for (int number : numbers) {
            if (number % 5 == 0) {
                System.out.print(number + " ");
            }
        }
        System.out.println();
    }
}

class AverageThread extends Thread {
    private int[] numbers;
    
    public AverageThread(int[] numbers) {
        this.numbers = numbers;
    }
    
    public void run() {
        int sum = 0;
        for (int number : numbers) {
            sum += number;
        }
        double average = (double) sum / numbers.length;
        System.out.println("Average: " + average);
    }
}

public class ThreadExample {
    public static void main(String[] args) {
        NumberInputThread inputThread = new NumberInputThread();
        inputThread.start();
        
        try {
            inputThread.join(); // Wait for the input thread to finish
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        
        int[] numbers = inputThread.getNumbers();
        
        DivisibleByFiveThread divisibleByFiveThread = new DivisibleByFiveThread(numbers);
        AverageThread averageThread = new AverageThread(numbers);
        
        divisibleByFiveThread.start();
        averageThread.start();
    }
}
