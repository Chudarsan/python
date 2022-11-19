Q1. Why do we call Python as a general purpose and high-level programming language?
	
	Python is general purpose language bcz it can use in various domain like web development, data science, AI, Financial etc
	Python is high-level programming language becauese its easy to use, runs on on any platofrom, has extensve support of libraries and easy to learn
	
Q2. Why is Python called a dynamically typed language?

	In python while declaring variables no need to specify type of the variable, which can be determined during run time. This makes python is dynamically typed language
	
Q3. List some pros and cons of Python programming language?
	
      Pros:
  
		Python is easy to learn and to use
		Supports multiple systems and platforms.
		supports Object-Oriented design.
		python has a variety  of frameworks that make web programming very flexible.
		Quick developement
		Extensive libraries are availbe for python
    
       Cons:
		Python is slow
		Python is not a very good language for mobile development.
		Python is not a good choice for memory intensive tasks.
		Has limitations with database access.
		Python is not good for multi-processor/multi-core work.
	
Q4. In what all domains can we use Python?

	Machine learning / Artificial intelligence
	Data analytics and data visualization 
	Web development
	Game development
	Mobile app development
	Embedded systems
	
Q5. What are variable and how can we declare them?

	Variables are the basic unit of storage in a programming language. By following syntax we declare varibles.
	language = 'Python' # here we can access 'Python' value location by using language
	
Q6. How can we take an input from the user in Python?

    By using input() built in function

Q7. What is the default datatype of the value that has been taken as an input using input() function?
	
	String --> str 
	
Q8. What is type casting?

	converting one type data tyoe to another data type
	
	ex: str_var = "100"
		int_var = int(str_var))
	
Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?

	Default data type of input is string, input wil be  one. However input can be taken in the form of some pattern
	and split() function to get multiple values
	ex: 	
	   str_ip = input("Enter numbers with space");
	   a,b,c = str_ip.split();
	   print("a value ",a)
	   print("b value ",b)
	   print("c value ",c)
	   
	o/p: Enter numbers with space 1 2 3
		 a value 1
		 b value 2
		 c value 3
	
Q10. What are keywords?

	Python has a set of keywords that are reserved words that cannot be used as variable names, function names, or any other identifiers

Q11. Can we use keywords as a variable? Support your answer with reason.

	No, keywords already defined by python for predefined functionality.if keywords used as varibles, it will throw 
	ex: 
	  and = 1;
	 o/p:
		syntax errors
		  File "/config/workspace/test.py", line 1
		and = 1;
		^
		SyntaxError: invalid syntax

Q12. What is indentation? What's the use of indentaion in Python?

	Indentation refers to the spaces at the beginning of a code line.
	Python indentation is a way of telling a Python interpreter that the group of statements belongs to a particular block of code.
	ex:
		if true:
			//statemet1 belongs to if block
			//atatement2 to if block
		else:
			//statemet3 belongs to else block 
		
Q13. How can we throw some output in Python?

	By using print() function we can print ouput to console.

Q14. What are operators in Python?

	The operator can be defined as a symbol which is responsible for a particular 
	operation between two operands
	ex: 
		numeric operators(+,-,*,/,**,%)
		assignment operators ( += ,-= ..)
		logical/boolean operators (and , or  not)
		
Q15. What is difference between / and // operators?

	/ --> for flot divson i.e will give decimal points also as output
	// --> for int divison
	ex: 
		print(5/3) --> 1.6666666666666667
		print(5/3) --> 1

Q16. Write a code that gives following as an output.
     iNeuroniNeuroniNeuroniNeuron

	print('iNeuron'*4)
		
Q17. Write a code to take a number as an input from the user and check if the number is odd or even.
	
	ip_num = int(input("Enter a number "))
	if (ip_num% 2 == 0):
		print(ip_num, " is a even number")
	else:
		print(ip_num, " is a odd number")
	
Q18. What are boolean operator?

    and, or , not

Q19. What will the output of the following?

	1 or 0 --> 1

	0 and 0 --> 0

	True and False and True --> False

	1 or 0 or 0 --> 1

Q20. What are conditional statements in Python?

	 if,else,elif
	 
Q21. What is use of 'if', 'elif' and 'else' keywords?
	
	 if', 'elif' and 'else' will be used to execute a certain line of codes based on  conditions
	 
Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".
	
	ip_age = int(input("Enter a Age "))
	if (ip_age >= 18):
		print("I can vote")
	else:
		print("I can't vote")
		
Q23. Write a code that displays the sum of all the even numbers from the given list.
	numbers = [12, 75, 150, 180, 145, 525, 50]
	
	program:
	
	numbers = [12, 75, 150, 180, 145, 525, 50]

	#by using iterative way
	result_sum = 0
	for num in numbers:
		result_sum += num;
	print("Sum of numbers in list = ",result_sum)

	# by using buit in function
	print("Sum of numbers in list = ",sum(numbers))



Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.

	prograam:
		ip_nums = input("Enter three numbers wseperated by space ")
		a,b,c = ip_nums.split()

		if (a >= b) and (a >= c):
			print(a ," is greatest number")
		elif (b >= a) and (b >= c):
		  print(b ," is greatest number")
		else:
			print(c ," is greatest number")
		
Q25. Write a program to display only those numbers from a list that satisfy the following conditions

The number must be divisible by five

If the number is greater than 150, then skip it and move to the next number

If the number is greater than 500, then stop the loop

numbers = [12, 75, 150, 180, 145, 525, 50]

	program:
		numbers = [12, 75, 150, 180, 145, 525, 50]

		for num in numbers:

			if num > 500:
				break
			elif num > 150:
				continue

			if (num % 5 == 0):
				print(num ," is divisible by 5")
		
Q26. What is a string? How can we declare string in Python?

     String is sequence of characters in python.
	 str_var = 'python'
		or
	 str_var = "Python"

Q27. How can we access the string using its index?

     By using [] and passingi index numer in it.
	 ex:
		str_var = "Python"
		print(str_var[3]) --> h

Q28. Write a code to get the desired output of the following
string = "Big Data iNeuron"
desired_output = "iNeuron"

	 program:
		 string = "Big Data iNeuron"
		 print(string[9:])

Q29. Write a code to get the desired output of the following
    string = "Big Data iNeuron"
    desired_output = "norueNi"

	program:
	
		string = "Big Data iNeuron"
		print(string[-1:-8:-1])

Q30. Resverse the string given in the above question.

	program:
		string = "Big Data iNeuron"
		print(string[-1::-1])
	
Q31. How can you delete entire string at once?

	 By using del keyword we can delete string from memory on python
	 del string
	 
Q32. What is escape sequence?

	Escape sequence is a sequence of characters with special meaning when used inside a string or a character.
	And  escape sequence charcters are non-printable when backslash preceds them.
	examples of escape sequences are \t,\b ,\n ...
	
	ex:
	print("Big\tData") --> here \t escape sequnece means tab. 
	o/p: Big	Data
	
Q33. How can you print the below string?
'iNeuron's Big Data Course'

   program:
    print("'iNeuron's Big Data Course'")
	
Q34. What is a list in Python?

	 List is one data type in python.
	 List can be used to store hetrogeneous or homogeneous kind of data
	 List will store sequential data
	 List will store data in contiguous memory location
	 ex: 
	 int_num = [2,3,4,5,6,7,8]
	 list1= [1,"python",5.0, True,]
	 
Q35. How can you create a list in Python?

	 By using [] or list()
	 ex:
	 list1 = []; #empty list
	 list2 = list() #empty list
	list3 = [3,"python",4.5,True] #list creation with data
	
Q36. How can we access the elements in a list?

	 List in python will store data in sequenetail manner, elemnts can access by using index
	 ex:
	 list1 = [2,"BigData", False]
	 list1[1] --> will return second element from list i.e "BigData"
	 
Q37. Write a code to access the word "iNeuron" from the given list.
lst = [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]

	lst[4][2]
	
Q38. Take a list as an input from the user and find the length of the list.

	 By using len() built in function list lenght can be found
	 ex: len(list1)
	 
Q39. Add the word "Big" in the 3rd index of the given list.
lst = ["Welcome", "to", "Data", "course"]

  	lst.insert(2, "Big")

Q40. What is a tuple? How is it different from list?

	tule is same as list , but it is non-modifiable. 
	we can only acccess values from tuple, but  can not insert, delete or assign values 
	
Q41. How can you create a tuple in Python?

	tuple1 = () #empty tuple
	tuple2 = tuple()#empty tuple
	tuple3 = (1,2,"python",True) # with data

Q42. Create a tuple and try to add your name in the tuple. Are you able to do it? Support your answer with reason.

	No, once tuple created we can not append elements to it.
	
Q43. Can two tuple be appended. If yes, write a code for it. If not, why?

        we can't add elements to a tuple because of their immutable property. 
	There's no append() or extend() method for tuples.
	
Q44. Take a tuple as an input and print the count of elements in it.

	By using len() bult in function , tuple lenght can be found
	len(tupl1)
	
Q45. What are sets in Python?

	A Set is an unordered collection data type that is iterable, mutable and has no duplicate elements
	
Q46. How can you create a set?

	 set1 = set() #empty set
	 set2 = {1,2,4,5,6,7} # with elements
	
Q47. Create a set and add "iNeuron" in your set.

	set1 = set() #empty set
	set1.add("iNeuron")
	
Q48. Try to add multiple values using add() function.

	set1 = set() #empty set
	set1.add("iNeuron")
	set1.add("Big data")
	set1.add("Course")
	
Q49. How is update() different from add()?

	 By using add we can add only one element to set
	 By using update we can add more than one element at a time  y uing list or set.
	 
	 ex:
		set1 = set() #empty set
		set1.add("iNeuron")
		set1.add("Big data")
		set1.add("Course")
		set1.update(['welcome','to','the','enginerring'])
	 
Q50. What is clear() in sets?

	 Remove all elements from this set
	 
Q51. What is frozen set?

	frozenset is an immutable Set
	
Q52. How is frozen set different from set?

	 Set is mutable and frozenset is immutable.
	 Set can be modified after creation, i.e append , remove, update .. operations are valid
	 frozenset can not be modified once its created. i.e append , remove, update .. operations can not  perform

Q53. What is union() in sets? Explain via code.

	 The union of two sets will give a new set that contains distinct elements from both sets.
	ex:
	  set1 = {1,4,6,7,8}
		set2 = {2,1,3,0,11,5}
		set3 = set1.union(set2)
		print(set3)
	o/p:
	   {0, 1, 2, 3, 4, 5, 6, 7, 8, 11}

Q54. What is intersection() in sets? Explain via code.

	  The intersection method of two sets will give new set containing the common elements of both the given sets
	  ex:
	    set1 = {1,4,6,7,8}
		set2 = {2,1,3,0,11,5,6}
		set3 = set1.intersection(set2)
		print(set3)
	o/p:
		{1, 6}
		
Q55. What is dictionary in Python?

	The dictionary is the data type in Python.By using dictionary we can store data in a key-value pair format
	ex: 
		person = { 'name': 'sudarsan', 'age':27,'email':'test@gmail.com'}
		
Q56. How is dictionary different from all other data structures.

	dictionary can be used store data in key-value format, where as other data structure data types can store only one value as the element
	
Q57. How can we delare a dictionary in Python?

     we can declare dictionary by using {} or dict() constructor
	 ex:
		dict1 = {} #empty dictionary
		dict2 = dict() #empty dictionary
		person = { 'name': 'sudarsan', 'age':27,'email':'test@gmail.com'} #dictiionary with values

Q58. What will the output of the following?
var = {}
print(type(var))

	<class 'dict'>
	
Q59. How can we add an element in a dictionary?

	 By Using [key] we can add elements to dictionary:
	 ex:
		person = {  'firstname': 'Sudarsan', 'age':27,' email':'test@gmail.com'} #dictiionary with values
		print(person)
		person['lastname'] = 'Reddy'
		print(person)
	o/p:
		{'firstname': 'Sudarsan', 'age': 27, ' email': 'test@gmail.com'}
		{'firstname': 'Sudarsan', 'age': 27, ' email': 'test@gmail.com', 'lastname': 'Reddy'}

Q60. Create a dictionary and access all the values in that dictionary.

	program:
		person = {'firstname': 'Sudarsan', 'age': 27, ' email': 'test@gmail.com', 'lastname': 'Reddy'}

		for key,value in person.items():
			print("key=",key,",value=",value)
		
Q61. Create a nested dictionary and access all the element in the inner dictionary.

	program:
		person = {'firstname': 'Sudarsan', 'address': {'house_no':45, 'street':'17 lane road','pincode':12345}, 'lastname': 'Reddy'}
		print(person['address'])
		for key,value in person['address'].items():
			print("key=",key,",value=",value)
		
Q62. What is the use of get() function?

	 The get() method can be used to get value by using key from dictionary.
	 ex:
		person = {'firstname': 'Sudarsan', 'lastname': 'Reddy'}
		person.get('firstname')
		
Q63. What is the use of items() function?

	The items() method can bu used to get key-value pairs of the dictionary in iterative way.
	ex:
		person = {'firstname': 'Sudarsan', 'address': {'house_no':45, 'street':'17 lane road','pincode':12345}, 'lastname': 'Reddy'}
		print(person['address'])
		for key,value in person['address'].items():
			print("key=",key,",value=",value)
			
Q64. What is the use of pop() function?

	 The  pop() method is used to removes the  key-value pair by using key from dictionary
	 
Q65. What is the use of popitem() function?

     The  popitem() removes the last inserted key-value pair from the dictionary dictionary (LIFO (last-in, first-out) order )
	 
Q66. What is the use of keys() function?

	 The keys() can be used to get all keys from dictionary
	 ex:
		person = {'firstname': 'Sudarsan', 'lastname': 'Reddy','age':27}
		print(person.keys()) 
	 o/p :
		dict_keys(['firstname', 'lastname', 'age'])

Q67. What is the use of values() function?

	The values() can be used to get all values from dictionary
	ex:
		person = {'firstname': 'Sudarsan', 'lastname': 'Reddy','age':27}
		print(person.values())
	o/p:
		dict_values(['Sudarsan', 'Reddy', 27])
		
Q68. What are loops in Python?

    Loops can be used to repeate something over and over until a particular condition is satisfied.

Q69. How many type of loop are there in Python?

	 The are two types of loops are there in python.
	 1) for loop
	 2) While loop
	 
Q70. What is the difference between for and while loops?

	For loop is used when the number of iterations is already known.
	While loop is used when the number of iterations is already Unknown.
	
Q71. What is the use of continue statement?

	A continue statement ends the current iteration of a loop and continue to next iteration.
	
Q72. What is the use of break statement?

	A break statement ends the loop 
	
Q73. What is the use of pass statement?

	The pass statement is used as a placeholder for future code. When the pass statement is executed, nothing happens, 
	but it will avoid getting an error when empty code is not allowed.
	ex:
	    if True:
	      #empty code will give error
	    print("end of the program")
		
		if True:
			pass: #empty code, but it will not give any error
			
	    print("end of the program")
	
Q74. What is the use of range() function?

	The range() function returns a sequence of numbers, starting from 0 by default,
	and increments by 1 (by default), and stops before a specified number.
	ex:
	   for num in rang(1,10): # will return 1,2,3,4,5,6,7,8,9 numbers in sequnce manner
	       print(num)
		   
Q75. How can you loop over a dictionary?

	 program:
			person = {'firstname': 'Sudarsan', 'address': {'house_no':45, 'street':'17 lane road','pincode':12345}, 'lastname': 'Reddy'}
			print(person['address'])
			for key,value in person['address'].items():
				print("key=",key,",value=",value)
	 
Coding problems

Q76. Write a Python program to find the factorial of a given number.

	  program:
			def factorial_iterative(num):

				if(num == 0 or  num == 1):
					return 1;

				factorial = 1
				for i in range(num,0,-1):
					factorial *= i;

				return factorial;

			print("iterative : ",factorial_iterative(10))

			def factorial_rescursive(num):

				if(num == 0 or  num == 1):
					return 1;

				return num * factorial_rescursive(num-1);


			print("resursive :: ",factorial_rescursive(10))
			
Q77. Write a Python program to calculate the simple interest. Formula to calculate simple interest is SI = (PRT)/100

	 program:
			def simple_interest(principle,rate_of_interest,tenure):
				si = (principle*rate_of_interest*tenure)/100
				print("Simple interest is = ",si)

			simple_interest(100000,2,1)
			
Q78. Write a Python program to calculate the compound interest. Formula of compound interest is A = P(1+ R/100)^t.

	 program:
	 
	 def compound_interest(principle,rate_of_interest,tenure):
		 amount = principle*(1 + rate_of_interest/100)**tenure
		 CI = amount - principle
		 print("Compound Interest = ",CI)

	compound_interest(10000, 10.25, 5)
	
Q79. Write a Python program to check if a number is prime or not.

	program:
		def prime_number(num):
			is_prime = True;
		   
			for i in range(2,(num//2)+1):
				if num % i == 0:
					is_prime =  False;
					break
			if is_prime:
				print(num," is a prime number")
			else:
				 print(num," is not a prime number")

	    prime_number(5)
		
Q80. Write a Python program to check Armstrong Number.

	 program:
		 def armstrong_number(num):
		   tmp_num = num
		   digit_sum = 0
		   while tmp_num > 0:
			digit = tmp_num % 10
			digit_sum += digit**3
			tmp_num = tmp_num // 10
		   if num == digit_sum :
			print(num , " is armstrong number")
		   else:
			 print(num , " is not armstrong number")

		 armstrong_number(153)

Q81. Write a Python program to find the n-th Fibonacci Number.

	program:
		def nth_fibonacci_num(n):
			if n < 0:
			   print(n , " should be greater than 0")
			   return
			elif n == 0:
				return 0
			elif n == 1:
				return 1

			first = 0
			second = 1

			for num in range(2,n+1):

				tmp =  first + second
				first = second
				second = tmp

			return second

		print(nth_fibonacci_num(10))

Q82. Write a Python program to interchange the first and last element in a list.

	program:
		num_list = [1,2,3,4,5,6,7,8,9,10]
		tmp = num_list[0]
		num_list[0] = num_list[len(num_list)-1 ]
		num_list[len(num_list)-1 ] = tmp
		print(num_list)
		
Q83. Write a Python program to swap two elements in a list.

	 def swap_two_elements_in_list(lst, pos1, pos2):
		first_element, second_elemnt = lst[pos1],lst[pos2]
		lst[pos1] = second_elemnt
		lst[pos2] = first_element
		return lst

	num_lst =  [1,2,3,4,5,6,7,8,9,10]
	swapped_lst = swap_two_elements_in_list(num_lst,5,9)

Q84. Write a Python program to find N largest element from a list.
```
        ip_lst = [10, 15, 20, 70]

	def n_largest(ip_lst, n):
	    op_list = []
	    for i in range(0, n):
		max_ele = 0
		for j in range(len(ip_lst)):
		    if ip_lst[j] > max_ele:
			max_ele = ip_lst[j];
		ip_lst.remove(max_ele);
		op_list.append(max_ele)
	    return op_list[n-1]

	print(n_largest(ip_lst,2))
```	
Q85. Write a Python program to find cumulative sum of a list.

	 program:
		num_lst =  [1,2,3,4,5,6,7,8,9,10]

		def sum_of_list_eleements(lst):
			sum = 0
			for i in lst:
				sum += i
			return sum

		print(sum_of_list_eleements(num_lst))
		
Q86. Write a Python program to check if a string is palindrome or not.

	 program:
		ip_str = 'Was it a car or a cat I saw'
		def is_palindrome_string_iterative(ip_str):
			op_str = ip_str.lower().replace(' ', '')
			first, second = 0, len(op_str) -1
			while first < second:
				if op_str[first] == op_str[second]:
					first += 1
					second -=1
				else:
					return False
			return True

		if is_palindrome_string_iterative(ip_str):
			print(ip_str,"is palindrome string")
		else:
			 print(ip_str," is not palindrome string")

		#recursive way
		def is_palindrome_string_recursive(ip_str):
			op_str = ip_str.lower().replace(' ', '')
			if len(op_str) <= 1:
				return True

			if op_str[0] == op_str[-1]:
				return is_palindrome_string_recursive(op_str[1:-1])
			else:
				return False

		if is_palindrome_string_recursive(ip_str):
			print(ip_str,"is palindrome string")
		else:
			 print(ip_str," is not palindrome string")
			 
Q87. Write a Python program to remove i'th element from a string.

	 def remove_ith_elm_from_string(ip_str,index_position):
		op_str = ip_str[0:index_position] +  ip_str[index_position+1:]
		
		return op_str

	print(remove_ith_elm_from_string('abcghh',0))
	
Q88. Write a Python program to check if a substring is present in a given string.

	 def is_substring(ip_str:str,sub_str:str):
		if ip_str.find(sub_str) > 0:
			return True
		else:
			return False

	print(is_substring('abcdffhj','fhj'))
	
Q89. Write a Python program to find words which are greater than given length k.

	 def words_greater_tahn_given_length(ip_str:str, length: int):
		words_lst = []
		for word in ip_str.split(" "):
			if len(word) >= length:
				words_lst.append(word)
		return words_lst

	 print(words_greater_tahn_given_length("a b v cf vgg d vbn fffri",2))
	 
Q90. Write a Python program to extract unquire dictionary values.


	program:
		def extract_unique_dict_values(ip_dict:dict):
			return set(ip_dict.values())

		ip_dict = {'Sachin': 10, 'MSD': 7, 'Kohli': 18, 'Rohit': 45, 'Jadeja': 10, 'Faf': 45}

		print(extract_unique_dict_values(ip_dict))
	
Q91. Write a Python program to merge two dictionary.

	program:

		d1 = {'a': 100, 'b': 200}
		d2 = {'x': 300, 'b': 400,'z':500}

		def merge_dict(d1:dict,d2:dict):
		   d3 = dict(d1)
		   for key,value in d2.items():
			if key in d3 :
				print(d3)
				d3[key] = [d3[key],value]
			else:
				 d3[key] = value
		   return d3

		print(merge_dict(d1,d2))
Q92. Write a Python program to convert a list of tuples into dictionary.
Input : [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
Output : {'Sachin': 10, 'MSD': 7, 'Kohli': 18, 'Rohit': 45}

	program:
		def convert_list_of_tuples_into_dictionary(lst_tuples):
		op_dict = {}
		for tuple_elm in lst_tuples:
			op_dict[tuple_elm[0]] = tuple_elm[1]
		return op_dict

	   ip_lst = [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
	   op_dict = convert_list_of_tuples_into_dictionary(ip_lst)
	   print(op_dict)
	   
Q93. Write a Python program to create a list of tuples from given list having number and its cube in each tuple.

Input: list = [9, 5, 6]
Output: [(9, 729), (5, 125), (6, 216)]

	program:
		  def convert_list_into_tuple_list_of_cubes(ip_lst):
			  op_tup_lst = []
			  for num in ip_lst:
				  op_tup_lst.append((num,num**3))
			  return op_tup_lst

		  ip_list = [9, 5, 6]
		  op_tup_lst = convert_list_into_tuple_list_of_cubes(ip_list)
		  print(op_tup_lst)

Q94. Write a Python program to get all combinations of 2 tuples.

Input : test_tuple1 = (7, 2), test_tuple2 = (7, 8)
Output : [(7, 7), (7, 8), (2, 7), (2, 8), (7, 7), (7, 2), (8, 7), (8, 2)]

     program:
	 def combination_of_two_tuples(tuple1:tuple, tuple2:tuple):
		 op_lst = []
		 for t1 in tuple1:
			 for t2 in tuple2:
				 op_lst.append((t1,t2))
		 for t1 in tuple2:
			 for t2 in tuple1:
				 op_lst.append((t1,t2))
		return op_lst

	 test_tuple1 = (7, 2)
	 test_tuple2 = (7, 8)

	 print(combination_of_two_tuples(test_tuple1,test_tuple2))
	 
	 
Q95. Write a Python program to sort a list of tuples by second item.

Input : [('for', 24), ('Geeks', 8), ('Geeks', 30)] 
Output : [('Geeks', 8), ('for', 24), ('Geeks', 30)]

	program:
		ip_lst = [('for', 24), ('Geeks', 8), ('Geeks', 30)] 

		def sort_key(ip_tuple1):
			return ip_tuple1[1]

		ip_lst.sort(key=sort_key)
		print(ip_lst)

Q96. Write a python program to print below pattern.
```
* 
* * 
* * * 
* * * * 
* * * * * 
```
	program:
            for i in range(5):
		print("*",end =" ")
		for j in range(i):
			print(" *",end =" ")
		print()
		
		
Q97. Write a python program to print below pattern.
```
    *
   **
  ***
 ****
*****  
```
	program:
		for i in range(5):
		    for j in range(5,0,-1):
		        if(j > i+1):
			    print(" ",end =" ")
			else:
		            print("*",end =" ")
		 print()
		
Q98. Write a python program to print below pattern.
```
    * 
   * * 
  * * * 
 * * * * 
* * * * * 
```
	program:
	   for i in range(5):
	       for k in range( 5 - (i+1)):
		   print(end =" ")

	       for j in range(i+1):
		   print("*",end =" ")
	       print()

Q99. Write a python program to print below pattern.
```
1 
1 2 
1 2 3 
1 2 3 4 
1 2 3 4 5
```
	program:

		for i in range(5):
		    for j in range(i+1):
			print(j+1,"",end =" ")
		    print()

Q100. Write a python program to print below pattern.
```
A 
B B 
C C C 
D D D D 
E E E E E 
```
	program: 

		for i in range(5):
		    for j in range(i+1):
			print(chr(65+i),"",end =" ")
		    print()
