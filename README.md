# Test1
Basics

			TEST-1
1.	What is the most important feature of java?
*Platform independent
*secure
*multithreading
*exception handing
*architectural neural
*real world objects
       2. What do you mean by platform independent?
Every hardware and software environment in which the program runs is called as platform. But java is a platform independent because JVM creates the source code into machine code. so that the class file run anywhere hence it is called as WORA (write once run anywhere).Java code can be run on multiple platforms.
      3. What is the difference between JVM,JDK and JRE?
JVM- java virtual machine which is used to translate the source code into machine level code
It has 2 functions. That is
*javac-java compiler
*java- interpreter  
		JRE-java runtime environment it implements the jvm ,and other .jre files.
		JDK-java development it consist of both  jvm and jre. but also includes development tools.
   4. What is the concept called Pointers? And does java supports Pointer?
pointing the variables address location. but java does not supports pointers because it is insecured one ,because  anyone can fetch the information with help of pointers. Java is a secured programming language, so it is isolated from pointers. 
   5. What is the base class of all the classes?
Extracting properties from the existing  things is called as inheritance. For an instance we can extract more subclasses. but the parent class is called as super class or base class.
Types:
	*single inheritance
	*multi level inheritance
*multiple inheritance(interface)
*hirarical inheritance
   6. What do you mean by local variables?
		*Local variables are placed in a method() only.
		* life time of the variables also within the method only.
*but it does not have a default value.
  7. What do you mean by class variables?
		*it access globally
		*it has default value
		*also known also instance variable.
	It have a static variable also.static is a key word but it access by a static method only.
 8. Can you explain: public static void main(String args[])
	It is a main method in java. By the way it will start the proceedings.
	*Public- executes access in any way.
	*Static-it does not need of creating objects.
	*Void-it does not return anything.
	*String agrs[]-commend line argumrnts means it stores the run time values to stored on it.
9. Can main method to be overloaded?
	No, we can’t pass arguments to main method.hence it does not allow overload.
10. Can a Class declared as protected?
	No, it does not support.it cause a error message.
11.I don’t want my class to be inherited by other classes. What should I do?
	*include class name before final keyword.
	*it does not allow inheritance and over ridding.

12.What is the purpose of declaring variable as final?
	*Through out the program it does not change the value.
	*because it initialized only once.
13.What is the impact of declaring a method as final?
	*cannot be override.
14. What is an abstract class and what is the purpose?
	When a method is decalred as abstract method means we have to put a class name before abstract keyword.if it’s a abstract class means it must be extend by sub class.
15.Can a abstract class defines as final?
	No. It does not allow because a class is a abstract class means it must be extend by someone.but final does not allow extends abstract and final not together.
16. Can you create object for abstract class
	No. But  we create a object  for sub class extended by abstract class.
	A-abstract class
	b-extend by a
	A s=new b()
17. What is the use of instanceof operator?
	For a particular instance check whether the object is appropriated to the class.but  one object can be assign to muttilpe classes.
	A s=new a()
	Boolean d=a.instanceof(A);
18.What is an abstract method?
	*Super class it just declared
		ex. abstract void display();
*sub class it defines the implement details over superclass
	ex.void display()
{
System.out.println(“abstract method..”);
}
19. What are the different types of if statements available?
		*if
		*if..else
		*if..else if..else
		*nested..if
20.Please explain about all access modifiers in java?
	In a way to restrict access to class, variables and methods is called as access modifiers.
		*default
		*private
		*protected
		*public

 
Access modifiers	same class	Out side of class in same package	Out side of class in other package	Sub class in other package
default	yes	yes	no	no
private	yes	no	no	no
Public	yes	yes	yes	yes
protected	yes	yes	no	yes


1.Getting three inputs from the user and displaying which one is greater one.
import java.util.Scanner;
class if_else_if
{
public static void main(String args[])
{
Scanner s=new Scanner(System.in);
System.out.println("enter the a value:");
int a=s.nextInt();
System.out.println("enter the b value:");
int b=s.nextInt();
System.out.println("enter the c value:");
int c=s.nextInt();

if((a>b)&&(a>c))
{
	System.out.println("a is the biggest value");
}
else if((b>a)&&(b>c))
{
	System.out.println("b is the biggest value");
}
else if((c>a)&&(c>b))
{
	System.out.println("c is the biggest value");
}
else{
	System.out.println("all the values are same only");
}
}
}

2.Student Marks grade system.
import java.util.Scanner;
class if_else_if
{
public static void main(String args[])
{
Scanner s=new Scanner(System.in);
System.out.println("enter the tamil mark:");
int a=s.nextInt();
System.out.println("enter the english mark:");
int b=s.nextInt();
System.out.println("enter the maths mark:");
int c=s.nextInt();
int total=a+b+c;
int ave=total/3;
	if(ave>=90)
	{
	System.out.println("s grade");
	}
	else if(ave>=80)
	{
	System.out.println("a  grade");
	}
	else if(ave>=70)
	{
	System.out.println("b grade");
	}
	else if(ave>=60)
	{
	System.out.println("c grade");
	}
	else if(ave>=50)
	{
	System.out.println("e grade");
	}
	else{
	System.out.println("fail");
	}
}
}

3.sample program for abstract class and method concept?

abstract class ab
{
int a=5;
abstract void display();
}
class ac extends ab
{
void display()
{
System.out.println("we are in a abstract method....");
}
}
class test
{
public static void main(String args[])
{
ab t1=new ac();
t1.display();
}
}


4.Sample program for swapping two variables without using third variable?
import java.util.Scanner;
class swap
{
	public static void main(String args[])
	{
		Scanner s=new Scanner(System.in);
		System.out.println("enter the a value");
		int a=s.nextInt();
		System.out.println("enter the b value");
		int b=s.nextInt();
		System.out.println("before swap:");
		System.out.println("a:"+a);
		System.out.println("b:"+b);
		a=a+b;
		b=a-b;
		a=a-b;
		System.out.println("\n");
		System.out.println("after swap:");
		System.out.println("a:"+a);
		System.out.println("b:"+b);
	}
}







