import java.util.concurrent.locks.ReentrantLock;

class BankAccount {
    private double balance;
    private ReentrantLock lock;

    public BankAccount(double initialBalance) {
        balance = initialBalance;
        lock = new ReentrantLock();
    }

    public void deposit(double amount) {
        lock.lock();
        try {
            balance += amount;
            System.out.println("Deposited $" + amount + " - New Balance: $" + balance);
        } finally {
            lock.unlock();
        }
    }

    public boolean withdraw(double amount) {
        lock.lock();
        try {
            if (balance >= amount) {
                balance -= amount;
                System.out.println("Withdrawn $" + amount + " - New Balance: $" + balance);
                return true;
            } else {
                System.out.println("Insufficient funds for withdrawal: $" + amount);
                return false;
            }
        } finally {
            lock.unlock();
        }
    }

    public double getBalance() {
        return balance;
    }

    public boolean transfer(BankAccount targetAccount, double amount) {
        if (this == targetAccount) {
            System.out.println("Cannot transfer to the same account.");
            return false;
        }

        lock.lock();
        targetAccount.lock.lock();
        try {
            if (this.withdraw(amount)) {
                targetAccount.deposit(amount);
                System.out.println("Transferred $" + amount + " to another account.");
                return true;
            } else {
                System.out.println("Transfer failed.");
                return false;
            }
        } finally {
            lock.unlock();
            targetAccount.lock.unlock();
        }
    }
}

class CustomerThread extends Thread {
    private BankAccount account;

    public CustomerThread(BankAccount account) {
        this.account = account;
    }

    public void run() {
        account.deposit(1000); // Deposit $1000
        account.withdraw(500); // Withdraw $500
        double balance = account.getBalance(); // Check balance
        System.out.println("Current Balance: $" + balance);
    }
}

public class BankAccountExample {
    public static void main(String[] args) {
        BankAccount account = new BankAccount(1000);

        CustomerThread customer1 = new CustomerThread(account);
        CustomerThread customer2 = new CustomerThread(account);

        customer1.start();
        customer2.start();
    }
}
