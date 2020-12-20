# FLUTTER

## WEEK 3

### OOP CONCEPTS IN DART

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

