Q1. What is the purpose of Python's OOP?

	OOP is programming paradigm that uses classes and object in programming. By using this we can create
	real world entinties such as book , car, house etc. we can structure a program by bundling properties
	and behavours of a entity.

Q2. Where does an inheritance search look for an attribute?

	The child class will first search the attribute in its own class, if not, then search
	in its parent classes in depth-first, left-right order. This is called Method Resolution Order (MRO) in Python.
	MRO defines how Python searches for inherited methods.
	we can check MRO by using __mro__ attribute in class
	
Q3. How do you distinguish between a class object and an instance object?

	Class variables are declared inside a class but outside of any function. 
	Class variables can be accessesdirectly with class name.
	Instance variables are declared inside the constructor which is the __init__method.
	Instance variables can be accsses after initalization class only.
	
	Ex:
		class Book:
			type = "finction"
			def __init__(self,name):
				self.name = name
		print(Book.type) # valid for class varaibles
		print(Book("Inception").name) #valid instance varibales
		
	
Q4. What makes the first argument in a class’s method function special?

	The first parameter of class's method function is self, which is self reference to
	instance of class. By using self param we can assign or modify attribute values to a particular 
	instance of a class
	
Q5. What is the purpose of the init method?
	the __init__ method will  be used intialize a class attributes. It is also called as 
	constructor.
	
	ex:
		class Person:
			def __init__(self):
				self.city = "Bangalore"
				self.name = "Sudarsan Reddy"

			def __repr__(self):
				return "Name : {} , City : {} ".format(self.name,self.city)

		person = Person()
		print(person)
		
	
	
Q6. What is the process for creating a class instance?

	To intialize Class attributes and behaviours
  
	ex:
		class Person:
			def __init__(self):
				self.city = "Bangalore"
				self.name = "Sudarsan Reddy"

			def __repr__(self):
				return "Name : {} , City : {} ".format(self.name,self.city)

		person = Person()
		print(person)
		


Q7. What is the process for creating a class?

	By using class key word we can create a class.
	ex:
		class Person:
			def __init__(self):
				self.city = "Bangalore"
				self.name = "Sudarsan Reddy"
		
Q8. How would you define the superclasses of a class?

	By specifying Super class name while creating Child class.
	
	Ex:
	class Job:
		def __init__(self,name):
			self.name = name

		def task(self):
			print("Workking")

	class DataEngineer(Job): #Here Job is the super class for DtaEngineer class
		
		def task(self):
			print("Workking as Data Enginerr")
		   

Q9. What is the relationship between classes and modules?

	Classes in python are templates/blueptint of object which contain properties and functions
	Modules in python is a way of organizing code , whhich contains reusable functions, classes and varibles
	
Q10. How do you make instances and classes?

	 To create instances of a class, will call the class using class name
	 and pass the arguments to  __init__ method.
	 
Q11. Where and how should be class attributes created?

	Class Varaibles will be created inside class and out side of functions/methods. These varibles shared across all objects of the class
	Ex:
		class Student:
			count = 0
			def __init__(self):
				Student.count += 1   
				
Q12. Where and how are instance attributes created?

	Instance Varibles will be created for particular instance of Object. These varibles will be attached/assigned object insode Constructor
    Ex:
		class Student:
			def __init__(self, name, age): 
				self.name = name
				self.age = age
				
Q13. What does the term "self" in a Python class mean?

	"self" refers to current instance of class only and is used to access variables that belongs to the class.
	
Q14. How does a Python class handle operator overloading?
	
	The operator overloading in Python means providing custom behaviour for operators. This can be achieved in Python by implementing magic or special functions
	Ex1: 
		Sting supports "+" operator to concatenate two strings. 
		 "Data" + "Engineer"
		
	Ex2:
		class A:
			def __init__(self,a):
				self.a = a;
			def __add__(self,otherA):
				return self.a + otherA.a

		a1 = A(10)
		a2 = A(20)
		print(a1 + a2)
		
Q15. When do you consider allowing operator overloading of your classes?

	Whenver we want to support operators functionalities to a class , need to implement operator overloading for class
	
Q16. What is the most popular form of operator overloading?

	  Addition (+) Operator 
	  
Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code?
	
	Both inheritance and polymorphism are fundamental concepts of object oriented programming of Python
	
	
Q18. Describe three applications for exception processing.
	
	There are mainly three kinds of distinguishable errors in Python: syntax errors, exceptions and logical errors
	
Q19. What happens if you don't do something extra to treat an exception?
	
	When an exception occurred, if you don't handle it, the program terminates abruptly and the code past the line that caused
	the exception will not get executed.
	
Q20. What are your options for recovering from an exception in your script?

	try-except
	try-except-else
	try-except-finally
	
Q21. Describe two methods for triggering exceptions in your script.
	
	 By using raise keyword, exceptions will be thrown manually
		
Q22. Identify two methods for specifying actions to be executed at termination time, regardless of
	 whether or not an exception exists.
	 
	
	Finally block always executes irrespective of an exception being thrown or not.
	

Q23. What is the purpose of the try statement?
	 
	 The try block is used to check some code for errors i.e the code inside the try block will execute when there is no error in the program.
	 
Q24. What are the two most popular try statement variations?

	 try-expect
	 try-except-else
	 try-except-finally
	 try-except-else-finally
	 
Q25. What is the purpose of the raise statement?
	 
	 By using raise , we throw exceptionin python code
	 
Q26. What does the assert statement do, and what other statement is it like?
	
	In Python, the assert statement is used to continue the execution if the given condition evaluates to True.
	If the assert condition evaluates to False, then it raises the AssertionError exception with the specified error message.
   
Q27. What is the purpose of the with/as argument, and what other statement is it like?
	
	The with statement in Python is used for resource management and exception handling.
	
	ex:
		file = open('file-path', 'w') 
		try: 
			file.write('Lorem ipsum') 
		finally: 
			file.close() 
		Above python code can be replace with statement
		
		with open('file-path', 'w') as file: 
		file.write('Lorem ipsum') 
		
Q28. What are *args, **kwargs?

	 *args and **kwargs allow us to pass multiple arguments or keyword/named arguments to a function.
	 
	 Ex:
		def sum(*args):
			result = 0
			for x in args:
				result += x
			return result

		print(sum(1, 2, 3))
	
		def concatenate(**kwargs):
			result = ""
			# Iterating over the Python kwargs dictionary
			for arg in kwargs.values():
				result += arg
			return result

		print(concatenate(a="Real", b="Python", c="Is", d="Great"))
		
		
Q29. How can I pass optional or keyword parameters from one function to another?
	
	 By assigning default values to the arguments we can set those arguments are optional
	 Ex:
  
		 def comp(a, b=2):
			if(a < b):
				print("first parameter is smaller")
			if(a > b):
				print("second parameter is smaller")
			if(a == b):
				print("both are of equal value.")
		 
		 
		print("first call")
		comp(1)
		print("second call")
		comp(2, 1)
		print("third call")
		comp(b=1, a=-1)
		print("fourth call")
		comp(-1, b=0)
  
Q30. What are Lambda Functions?

	 Lambda functions are the unnamed functions. Lambda functions can be crated with def keyword
	 Ex:
		sum = lambda x,y : x+y
		print(sum(1,2))

Q31. Explain Inheritance in Python with an example?
	
	The method of inheriting the properties of parent class into a child class is known as inheritance. It is an OOP concept. Following are the benefits of inheritance.

		* Code reusability- we do not have to write the same code again and again, we can just inherit the properties we need in a child class.

		* It represents a real world relationship between parent class and child class.

		* It is transitive in nature. If a child class inherits properties from a parent class, then all other sub-classes of the child class will also inherit the properties of the parent class.
	Ex:
		class Parent():
			def first(self):
			   print('first function')
 
		class Child(Parent):
		    def second(self):
			   print('second function')
		 
		ob = Child()
		ob.first()
		ob.second()
		
Q32. Suppose class C inherits from classes A and B as class C(A,B).Classes A and B both have their own versions of method func(). If we call func() from an object of class C, which version gets invoked?
	
	As per MRO in python A class func() will be called
	
Q33. Which methods/functions do we use to determine the type of instance and inheritance?

	 isinstance() and issubclass() are used to check inheritances. 
	 The function isinstance() returns True if the object is an instance of the class
	 The function issubclass() returns True if the Class is Derived from its parent class
	 Ex:
		class Parent():
			def first(self):
				print('first function')

		class Child(Parent):
			def second(self):
				print('second function')
			
		ob = Child()
		print(isinstance(ob, Parent))
		print(issubclass(Child, Parent))
		
Q34. Explain the use of the 'nonlocal' keyword in Python.

	 The nonlocal keyword is used to work with variables inside nested functions, where the variable should not belong to the inner function.
	 
	Ex:
		def nonLocalFun():
		x = 10
		# Nested Function
		def g():
			nonlocal x
			x = 1
			def h():
				nonlocal x
				print(x)
				x = 20
			h()
			print(x)
		g()
		print (x)
		
		nonLocalFun()

Q35. What is the global keyword?

	 Varibles declared out side of all functions called as global varibles
	 global keyword will be used to refer global scope varibles in non global scope
	 
	 Ex:
		globalVariable = 200;
		def withoutGlobalKeyWord():
			globalVariable = 500; # local to withoutGlobalKeyWord function
			print(globalVariable) # 500
		print(globalVariable) # 200
		withoutGlobalKeyWord()
		print(globalVariable)	# 200

		globalVariable = 200;
		def withGlobalKeyWord():
			global globalVariable # here we refering to global scope globalVariable
			globalVariable = 500 # here we modifying to global scope globalVariable
			print(globalVariable) # 500
		print(globalVariable) # 200
		withGlobalKeyWord()
		print(globalVariable) # 500
