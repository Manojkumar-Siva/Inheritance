# Inheritance

## Aim:
To write a C# program to print some messages using hierarchical inheritance.
## Algorithm:
### Step 1: 
Create a base class.

### Step 2: 
Create two child class.

### Step 3: 
Create a constructor in the base class and print a message.

### Step 4: 
Create a function in child class to print a message.

### Step 5: 
End the program.

## Program:
```
Developed by : Manoj Kumar S
Reg.no: 212221230056
```
```c#
using System;
public class tyre
{
    public tyre() {
        Console.WriteLine("Give the tyre type");
    }
    public virtual void display()
    {
        Console.Write("Tyre Type =");
    }
}
public class car : tyre
{
    public override void display()
    {
        base.display();
        Console.WriteLine("Car Tyre");
    }
}
public class scooter : tyre
{
    public override void display()
    {
        base.display();
        Console.WriteLine("Scooter tyre");
    }
}
public class program
{
    static void Main()
    {
        car c =new car();
        c.display();
        Console.WriteLine();
        scooter s=new scooter();
        s.display();
    }
}

```

## Output:
![Alt text](image.png)

## Result:
Thus C# program to print messages using hierarchical inheritance is written and executed sucessfully.