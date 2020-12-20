# FLUTTER

## WEEK 2

### BASICS OF DART

* Go to the [online editor](dartpad.dartlang.org) to practice the dart programming language.
    1. The console on the top-right is where the output will be printed.
    1. To run the code click *Run* which is highlighted on the top.
    
* To print Hello World:
```
void main() {
  print('hello world');
}
```
Here, main() is the main function.

#### DATATYPES-
1.Integer-for integer, non fractional values(int).

2.Double-for floating point numbers(double).

3.Strings-for sequence of characters(String).

4.Boolean-to represent boolean values-true or false(bool).

5.List and Map- to represent collection of ordered and unordered objects.

6.Dynamic-used as a type annotation explicitly(dynamic).

#### VARIABLES-
* Dart is a statically typed programming language i.e, when the variables are declared using a particular datatype it cannot be changed to another datatype in the future.

```
void main() {
  int age =15;
  age ='str';
  print(age);
}
```
The above code will throw the following error:

*Error: A value of type 'String' can't be assigned to a variable of type 'int'.*

* To overcome the above problem *Dart* uses dynamic datatype.

```
void main() {
  dynamic age =15;
  age ='str';
  print(age);
}
```

The above code will give the following output-

```
str
```

#### FUNCTIONS-

The syntax of the function-

```
return-type functionname()
{
  statements;
}
 ```
Another way of declaring a function when the function contains only one statement.
```
 return-type functionname() => statement;
 ```
Example Function call-

```
void main() {
  String n=name();
  int g=get();
  print(n);
  print(g);
}

String name(){
  return 'hi';
}

int get(){
  return 10;
}
```
The above code will give the following output-

```
hi
10
```
#### LISTS

It is similar to the lists in python programming language.

Ex-
```
void main() {
  List l1=[1,2,3];
  print(l1);
}
```
The above code will give the following output-

```
[1, 2, 3]
```
To add elements in the list, we can use `list_name.add(elements);` statement.

```
void main() {
  List l1=[1,2,3];
  l1.add(4);
  print(l1);
}
```

The above code will give the following output-

```
[1, 2, 3, 4]
```
To remove elements in the list, we can use `list_name.remove(elements);` statement.

```
void main() {
  List l1=[1,2,3];
  l1.remove(2);
  print(l1);
}
```
The above code will give the following output-

```
[1, 3]
```
Now that we have not mentioned a particular datatype for the list we can add variable of any datatype to a list of any datatype. So in order to avoid this practice we can mention the datatype to the list like the one done below:

```
void main() {
  List<int> l1=[1,2,3];
  print(l1);
}
```
The above code will give the following output-

```
[1, 2, 3]
```

#### CLASS

A blueprint for creatig objects.It is used to describe objects by giving them methods and properties.
* The syntax of the class-
```
class classname{
data members;
returntype methodname()
{
statements;
}
}
main()
{
classname objectname=classname();\\instantiating
}
```
Ex-
```
void main() {
  c1 c=c1();\\instantiating
  print(c.a);
  print(c.b);
  c.get();\\calling the method
}

class c1{
  String a="hi";
  int b=13;
  
  void get(){
    print('hello');
  }
}
```

The above code will give the following output-

```
hi
13
hello
```

CONSTRUCTORS-
It is invoked at the time of object creation.

```
classname(list of paramaters){
statemnets;
}
```

Ex-

```
void main() {
  c1 c=c1('hi',13);\\should be in same order as the constructor parameter list
  print(c.a);
  print(c.b);
  c.get();
}

class c1{
  String a;
  int b;
  c1(String a,int b)
  {
    this.a=a;\\using this keyword to initialise it to the same variable
    this.b=b;
  }
  void get(){
    print('hello');
  }
}
```
The above code will give the following output-

```
hi
13
hello
```
#### INHERITANCE

It is property to derive properties of the baseclass to subclass(class which extends).There are many types of inheritance in object oriented programming.

The syntax-

```
class subclassname extends baseclass{
statements;
}
```
Ex-

```
void main() {
  c1 c=c1('hi',13);
  print(c.a);
  print(c.b);
  c.get();
  c2 ce=c2('go',10);
  ce.put();
}

class c1{   \\baseclass
  String a;
  int b;
  c1(String a,int b)
  {
    this.a=a;
    this.b=b;
  }
  void get(){
    print('hello');
  }
}

class c2 extends c1{    \\subclass
  c2(String a,int b): super(a,b);
   void put(){
    print('hell');
  }
}
```
The above code will give the following output-

```
hi
13
hello
hell
```


