1. Student Class

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
