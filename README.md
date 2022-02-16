#  IOS DEVELOPMENT USING SWIFT 

----

## XCODE 
* PLAYGROUND :=> file -> new -> playground 
* LINE NO :=> XCODE -> prefrence -> editor -> line no 

---

## Keywords 
* declarations
```
Class	
deinit	
Enum	
extension
Func	
import	
Init	
internal
Let	
operator	
private	
protocol
public	
static	
struct	
subscript
typealias	
var
```
* statements
```
break	
case	
continue	
default
do	
else	
fallthrough	
for
if	
in	
return	
switch
where	
while
```
* expressions and types
```
as	
dynamicType	
false	
is
nil	
self	
Self	
super
true	
_COLUMN_	
_FILE_	
_FUNCTION_
_LINE_
```
* contexts
```
associativity	
convenience	
dynamic	
didSet
final	
get	
infix	
inout
lazy	
left	
mutating	
none
nonmutating	
optional	
override	
postfix
precedence	
prefix	
Protocol	
required
right	
set	
Type	
unowned
weak	
willSet
```

---

## Comments 
* single line comments 
```
  //  xxxxx
```
* multi line comments
```
/*    
   xxxxx
   xxxxx
*/
```

---

## Built-in Data Types 
* String 
	* var name:String = "xxx"
* Int 
	* var age:Int = 10
* Float 
	* var sal:Float = 20.2
* Double
	* var totalSal:Float = 200.22
* Bool 
	* var varName:Bool = true 
* Character
	* This is a single-character string literal.
* Optional
	* This represents a variable that can hold either a value or no value
* Tuples
	* This is used to group multiple values in single Compound Value

---

## Literals
* Integer Literals
	* let decimalInteger = 17         // 17 in decimal notation
	* let binaryInteger = 0b10001     // 17 in binary notation
	* let octalInteger = 0o21         // 17 in octal notation
	* let hexadecimalInteger = 0x11   // 17 in hexadecimal notation
* Floating-point Literals
	* let decimalDouble = 12.1875
	* let exponentDouble = 1.21875e1
	* let hexadecimalDouble = 0xC.3p0
* String Literals
	* let name = "xxxxxx"
* Boolean Literals
	* true
	* false
	* nil 

----

## Type Aliases
* create a new name for an existing type using typealias
	* typealias newname = type
	* typealias Feet = Int
		* var distance: Feet = 100

## Optional Value Diclaration 
* Optionals type, which handles the absence of a value
	* var intVar: Int?
	* var strVar: String?
	* var doubleVar: Double?

## Optional Binding
* optional binding to find out whether an optional contains a value, and if so, to make that value available as a temporary constant or variable
```
var someOptional:DataType?
someOptional = xxxxx
if let constantName = someOptional {
   statements
}
```

## NoValue 
* nil is used to represent no value 
	* var perhapsStr: String? = nil

## TypeConvertion 
* use the DataType class constructor for type converstion 
* var varName = DataType(otherTypeValue)
	* var number = String(12345)

---

## Variable 
* can hold value, reference to object or pointer to the function 
* var keyworld is used to diclar variable 
	* var varName = [initial value]
	* var varName:DataType = [initial value]
		* var name:String = " adarsh kumar "
		* var age:Int = 20

---

## Constents 
* let keyworld is used to diclare constant 
	* let constName  = [initial value]


## Printing Constants
* interpolate a variable value by wrapping the name in parentheses and escape
```
let name = "adarsh kumar"
let worth = 1000.00

print("Person who \(name) is more than \(worth) millions")

```
---

## print()
	* to print data on the console 

---

## Operators
* Arithematic operation 
	* \+	Adds two operands	A + B will give 30
	* −	Subtracts second operand from the first	A − B will give -10
	* \*	Multiplies both operands	A * B will give 200
	* /	Divides numerator by denominator	B / A will give 2
	* %	Modulus Operator and remainder of after an integer/float division	B % A will give 0
* Comparison Operators
	* ==	Checks if the values of two operands are equal or not; if yes, then the condition becomes true.	(A == B) is not true.
	* !=	Checks if the values of two operands are equal or not; if values are not equal, then the condition becomes true.	(A != B) is true.
	* \>		Checks if the value of left operand is greater than the value of right operand; if yes, then the condition becomes true.	(A > B) is not true.
	* <		Checks if the value of left operand is less than the value of right operand; if yes, then the condition becomes true.	(A < B) is true.
	* \>=	Checks if the value of left operand is greater than or equal to the value of right operand; if yes, then the condition becomes true.(A >= B) is not true.
	* <=	Checks if the value of left operand is less than or equal to the value of right operand; if yes, then the condition becomes true.	(A <= B) is true.
* Logical Operators
	* &&	Called Logical AND operator. If both the operands are non-zero, then the condition becomes true.	(A && B) is false.
	* ||	Called Logical OR Operator. If any of the two operands is non-zero, then the condition becomes true.	(A || B) is true.
	* !		Called Logical NOT Operator. Use to reverses the logical state of its operand. If a condition is true, then the Logical NOT operator will make it false.	!(A && B) is true.
* Assignment Operators
	* =	Simple assignment operator, Assigns values from right side operands to left side operand	C = A + B will assign value of A + B into C
	* +=	Add AND assignment operator, It adds right operand to the left operand and assigns the result to left operand	C += A is equivalent to C = C + A
	* -=	Subtract AND assignment operator, It subtracts right operand from the left operand and assigns the result to left operand	C -= A is equivalent to C = C - A
	* *=	Multiply AND assignment operator, It multiplies right operand with the left operand and assigns the result to left operand	C *= A is equivalent to C = C * A
	* /=	Divide AND assignment operator, It divides left operand with the right operand and assigns the result to left operand	C /= A is equivalent to C = C / A
	* %=	Modulus AND assignment operator, It takes modulus using two operands and assigns the result to left operand	C %= A is equivalent to C = C % A
	* <<=	Left shift AND assignment operator	C <<= 2 is same as C = C << 2
	* \>>=	Right shift AND assignment operator	C >>= 2 is same as C = C >> 2
	* &=	Bitwise AND assignment operator	C &= 2 is same as C = C & 2
	* ^=	bitwise exclusive OR and assignment operator	C ^= 2 is same as C = C ^ 2
	* |=	bitwise inclusive OR and assignment operator	C |= 2 is same as C = C | 2
* Range Operators
	* Closed Range	(a...b) defines a range that runs from a to b, and includes the values a and b.	1...5 gives 1, 2, 3, 4 and 5
	* Half-Open Range	(a..< b) defines a range that runs from a to b, but does not include b.	1..< 5 gives 1, 2, 3, and 4
	* One- sided Range	a… , defines a range that runs from a to end of elements …a , defines a range starting from start to a 1… gives 1 , 2,3… end of elements …2 gives beginning… to 1,2

* Misc Operators
	* Ternary Conditional	Condition ? X : Y	If Condition is true ? Then value X : Otherwise value Y	

## Operators Precedence
* Primary Expression Operators	() [] . expr++ expr--	            left-to-right
* Unary Operators				\* & + - ! ~ ++expr --expr           
								\* / %
								+ -
								\>> <<
								< > <= >=
								== !=								right-to-left
* Binary Operators				&	^	| &&	||					left-to-right
* Ternary Operator				?:									right-to-left
* Assignment Operators	        = += -= *= /= %= >>= <<= &=^= |=	right-to-left
* Comma							,									left-to-right


---

## Condition Statement 
* if statement
```
	if condition {

	}
```
* if else 
```
		if condition {

		} else {

		}
```
* if else if 
```
		if condition {

		} else if condition {

		}
```

* swtich case 
```
switch(expression){
   case constant-expression :
      statement(s);
      break; /* optional */
   case constant-expression :
      statement(s);
      break; /* optional */

   /* you can have any number of case statements */
   default : /* Optional */
      statement(s);
}
```
* fallthrough statement
```
switch expression {
   case expression1 :
      statement(s)
      fallthrough /* optional */
   case expression2, expression3 :
      statement(s)
      fallthrough /* optional */

   default : /* Optional */
      statement(s);
}
```

---

## Loops 
* for-in loop
	* iterates over collections of items, such as ranges of numbers, items in an array, or characters in a string
```
for index in var {
   statement(s)
}
```
* while loop 
```
while condition {
   statement(s)
}
```

* repeat...while loop
	* repeat...while loop is guaranteed to execute at least once.
```
repeat {
   statement(s);
} 
while( condition );
```
* Continue Statement
* Break Statement

---

## String 
* property 
	* isEmpty A Boolean value that determines whether a string is empty or not.
	* utf8 Property to return a UTF-8 representation of a string.
	* UTF-16 Property to return a UTF-16 representation of a string.
	* unicodeScalars Property to return a Unicode Scalar representation of a string.
	* startIndex	To get the value at starting index of string.
	* endIndex	To get the value at ending index of string.
	* Indices	To access the indeces one by one. i.e all the characters of string one by one.
* function 
	* hasPrefix(prefix: String) Function to check whether a given parameter string exists as a prefix of the string or not.
	* hasSuffix(suffix: String) Function to check whether a given parameter string exists as a suffix of the string or not.
	* toInt()	Function to convert numeric String value into Integer.
	* count() Global function to count the number of Characters in a string.
	* insert("Value", at: position)	To insert a value at a position.
	* remove(at: position)	removeSubrange(range)	to remove a value at a position, or to remove a range of values from string.
	* reversed()	returns the reverse of a string
	* append(string)
* operator 
	* \+ Operator to concatenate two strings, or a string and a character, or two characters.
	* +=	Operator to append a string or character to an existing string.
	* ==	Operator to determine the equality of two strings.
	* <	Operator to perform a lexicographical comparison to determine whether one string evaluates as less than another.
* String Interpolation
```
var name = "adarsh"
var age = 20
var message = "name and \(name)  age \(age) "
```

## Characters
	* let charVar: Character = "A"
	* print("Value of charVar \(charVar)")


---

## Arrays 
* var array = \[DataType\]()
* var array :[DataType]=[Elements]
* var array = [DataType](count:NumbeOfElements,repeatedValue:InitialValue)

* Accessing Arrays
	* arrayVar[index]
```
var array = [Int](count: 3, repeatedValue: 10)
print( "Value of second element is \(array[0])" )
print( "Value of second element is \(array[1])" )
print( "Value of third element is \(array[2])" )
```

* Modifying Arrays
	* arrayVar.append(valueOfType)
	* arrayVar[index]=valueOfType
```
var array = [Int]()
array.append(20)
array.append(30)
array += [40]
array[0]= 10 
print( "Value of second element is \(array[0])" )
print( "Value of second element is \(array[1])" )
print( "Value of third element is \(array[2])" )
``` 

* Iterating an Array
	* using loops 
```
var array = [Int]()
array.append(20)
array.append(30)
for item in array {
   print(item)
}
```

* Adding Two Arrays
	 * array1 + array2 
```
var array1 = [Int](count:2, repeatedValue: 2)
var array2 = [Int](count:3, repeatedValue: 1)

var array = array1 + array2
for item in array {
   print(item)
}
```

* Array Property 
	* array.count
	* array .isEmpty 
```
var array1 = [Int](count:2, repeatedValue: 2)
var array2 = [Int](count:3, repeatedValue: 1)

print("Total items in array1 = \(array1.count)")
print("Total items in array2 = \(array2.count)")
var array = [Int]()
print("is array empty = \(array.isEmpty)")
array = array1+array2
print("is array empty = \(array.isEmpty)")
print("Total items in array = \(array.count)")
```

---

## Sets
* store distinct values of same types without order preserve 
* var setVar = Set<DataType>() 
* property 
	* setVar.count 
	* setVar.isEmpty 
* method 
	* setVar.insert(typeValue)
	* setVar.remove(typeValue)
	* setVar.contains(typeValue)
	* setVar.sorted()

* Iterating on Set
	* using loop 
```
for items in setVar {
   print(item)
}
```
* operations 
	* Intersection
	* Union
	* subtracting
```
let evens: Set = [10,12,14,16,18]
let odds: Set = [5,7,9,11,13]
let primes = [2,3,5,7]

odds.union(evens).sorted()
// [5,7,9,10,11,12,13,14,16,18]

odds.intersection(evens).sorted()
//[]

odds.subtracting(primes).sorted()
//[9, 11, 13]
```

---

## Dictionaries
*  store unordered lists of values of the same type it used to store key value paire where key is identifier 
* var dicVar = \[KeyDataType: ValueDataType\]()
