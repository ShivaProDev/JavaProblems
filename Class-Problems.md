
# **Level 1: Basic Class Problems**
## **1. Student Class**

Create a class Student with:
rollNo name marks

Methods:
setData() displayData()

Sample Output
Roll No: 101 Name: Shiva Marks: 85

```java
class Student { 
    String rollNo; 
    String name; 
    int marks;

    void setData(String rollNo, String name, int marks) {
        this.rollNo = rollNo;
        this.name = name;
        this.marks = marks;
    }

    void displayData() {
        System.out.printf("Roll No : %s", this.rollNo).println();
        System.out.printf("Name : %s", this.name).println();
        System.out.printf("Marks : %d", this.marks).println();
    }
}

class Main { 
    public static void main(String[] args) { 
        System.out.println("Environment Started"); 
        Student studOne = new Student(); 
        Student studTwo = new Student(); 
        studOne.setData("4gk16", "Shiva", 100); 
        studTwo.setData("$gk17", "Kiran", 90); 
        studOne.displayData(); 
        studTwo.displayData(); 
    } 
}


```

## **2. Rectangle Class**

Create a class Rectangle.

Data members:

length
width

Methods:

calculateArea()
calculatePerimeter()

Expected

Area = 50
Perimeter = 30

```java
class Rectangle {

    int length;
    int width;

    public Rectangle(int length,int width){

        this.length = length;
        this.width = width;
        
    }

    int calculateArea(){
        int area = this.length * this.width;
        return area;
    }

    int calculatePerimeter(){
        int peri = 2 * (this.length+this.width) ;
        return peri;
    }
}

class Main {
    public static void main(String[] args) {
       System.out.println("Environment Started");
        Rectangle rectOne = new Rectangle(8,5);
        Rectangle rectTwo = new Rectangle(6,4);
        int rectOneArea = rectOne.calculateArea();
        int rectOnePeri = rectOne.calculatePerimeter();
        System.out.printf("Area = %d cm2",rectOneArea).println();
        System.out.printf("Perimeter = %d cm",rectOnePeri).println();
        int rectTwoArea = rectOne.calculateArea();
        int rectTwoPeri = rectOne.calculatePerimeter();
        System.out.printf("Area = %d cm2",rectTwoArea).println();
        System.out.printf("Perimeter = %d cm",rectTwoPeri).println();
        
    }
}

```

## **3. Bank Account**

Create a class BankAccount.

Variables:

accountNumber
holderName
balance

Methods:

deposit(amount)
withdraw(amount)
displayBalance()

```java

class BankAccount {

    int accountNumber;
    String holderName;
    int balance;

    public BankAccount(int accountNumber,String holderName,int balance){

        this.accountNumber = accountNumber;
        this.holderName = holderName;
        this.balance = balance;
        
    }

    void deposit(int amount){
         this.balance = this.balance + amount;
    }

    void withdraw(int amount){
        this.balance = this.balance - amount;
    }
    void displayBalance(){
        System.out.printf("Avaible balance is : %d",this.balance).println();
    }
}

class Main {
    public static void main(String[] args) {
       System.out.println("Environment Started");
        BankAccount AccuntOne = new BankAccount(12967,"Shiva",100);
        BankAccount AccuntTwo = new BankAccount(12968,"Kiran",500);
        AccuntOne.displayBalance();
        AccuntOne.deposit(100);
        AccuntOne.displayBalance();
        AccuntOne.withdraw(50);
        AccuntOne.displayBalance();
        
    
        
        
    }
}
```

# **Level 2: Constructors**
## **4. Employee Class**

Create a class Employee.

Variables:

id
name
salary

Create:

Default constructor
Parameterized constructor

Display employee details.

```java

class Employee {

    int id;
    String name;
    int salary;

     public Employee(){
          this.id = 1234;
        this.name = "Emp1";
        this.salary = 1000;
     }
    public Employee(int id,String name,int salary){

        this.id = id;
        this.name = name;
        this.salary = salary;
        
    }
    

    void displayEmployeeDetails(){
        System.out.printf("Employee  id is : %d and Employee name is: %s and Employee Salary is :%d",this.id,this.name,this.salary).println();
    }
}

class Main {
    public static void main(String[] args) {
       System.out.println("Environment Started");
        Employee EmployeeOne = new Employee(12967,"Shiva",100);
      
        EmployeeOne.displayEmployeeDetails();
        
        
    
        
        
    }
}
```







