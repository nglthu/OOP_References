# Code Platform for OOP

# Learn Java

[Java Toutorial](https://www.w3schools.com/java/default.asp)


# Simple Exercies

1. Main
```
//Import library, e.g for Date
import java.util.Date;
public class HelloWorld {
    // Declare main without returning any agruments
    public static void main(String[] args) {
    // Declare variable, e.g SiSoLop type of int
        int SiSoLop;
        SiSoLop = 40;
    // object d instance of Date
        Date d = new Date();
    // display e.g print out SiSoLop and Date 
        System.out.println(SiSoLop);
        System.out.println(d);
    }
}

```
2
```
class Number {
    public int i;
}
class HelloWorld {
    public static void main(String[] args) {
        Number n1 = new Number();
        Number n2 = new Number();
        n1.i = 2;
        n2.i = 5;
        n1.i = n2.i;
        n2.i = 10;	// what is n1.i?
        System.out.println(n2.i);//10
        System.out.println(n1.i);//5
    }
}


```
3
```
class Number {
    public int i;
}
class HelloWorld {
    public static void main(String[] args) {
        Number n1 = new Number();
        Number n2 = new Number();
        n1.i = 2;
        n2.i = 5;
        n1 = n2;
        n2.i = 10;	// what is n1.i?
        System.out.println(n1.i);//10
        n1.i = 20;	// what is n2.i?
        System.out.println(n2.i);//20
    }
}

```
4. Alias
```
class Number {
    public int i;
}
class HelloWorld {
     static void f(Number m) {
        m.i = 15;
    }
    public static void main(String[] args) {
        Number n1 = new Number();
        Number n2 = new Number();
        Number n = new Number();
        n1.i = 2;
        n2.i = 5;
        n1 = n2;
        n2.i = 10;	// what is n1.i?
        System.out.println(n1.i);//10
        n1.i = 20;	// what is n2.i?
        System.out.println(n2.i);//20
        n.i = 14;
        f(n);//// what is n.i now?
        System.out.println(n.i);//15
    }
}

```
