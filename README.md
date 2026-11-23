# OOp-Lab-Task-4

class Account {

    void displayInfo() {
        System.out.println("General Bank Account");
    }
}

class SavingsAccount extends Account {

    @Override
    void displayInfo() {
        System.out.println("Savings Account");
        System.out.println("Interest Rate: 5%");
    }
}

class CurrentAccount extends Account {

    @Override
    void displayInfo() {
        System.out.println("Current Account");
        System.out.println("No Interest Provided");
    }
}

public class Main {
    public static void main(String[] args) {

        Account a = new Account();
        SavingsAccount s = new SavingsAccount();
        CurrentAccount c = new CurrentAccount();

        System.out.println("Account Information:");
        a.displayInfo();

        System.out.println("\nSavings Account:");
        s.displayInfo();

        System.out.println("\nCurrent Account:");
        c.displayInfo();
    }
}
