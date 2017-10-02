1. 
a = 1 assigns the value for the variable a as the 8byte int number 1. 
b = 'x' assigns the value for the variable b as the 2byte char letter x. 
 c = true assigns the value for the variable c as the 1byte logical value true. 
whos a b c indicates the name of the variables a, b, and c as well as lists the number of bytes for each variable, and the class of each variable.
 a == c determines if a is equal to c. This is true because a=1 and c=logical which is also 1.
 a+c adds the variables a and c which are both of value 1 even though one is a number and the other is a logical, so 1 + 1 = .
 d = [1 2 3 4] assigns the value for the variable d as 1 x 4 array of 4 numbers each of 8 bytes so 4 * 8 = totally 32 bytes 
 e = ['a' 'b' 'c' 'd'] assigns the value for the variable e as 1 x 4 array of 4 characters each of 2 bytes so 4 * 2 = totally 8 bytes 
 f = ['abcd'] assigns the value for the variable f as 1 x 4 regular array of 4 characters and is identical to the variable 
 g = {'a' 'b' 'c' 'd'} assigns the value for the variable g as 1 x 4 cell array of values 
 h = { a b c d} constructs a cell array h of the variables a, b, c, and d 
whos d e f g h inficates the name, number of bytes, class, and attribbutes of the variables d, e, f, g,h 

 
2. Casting a larger number than the maximum value just changes its value to the maximum value. Going outside the bounds returns the bounds. 

The maximum value of int16 can be found through intmax('int16') which is 3276. intmin('int'16') finds -32768

The maximum value of int32 can be found by intmax which is 214748367 and intmin whic is -2147483648

3.
 1\2 gives you 2 divided by 1 which is 2 
 1/2 gives you 1/2 which is 0.5000 
int8(1/2) gives you 1/2 as an 8 bit integer which is 1, because it rounds up from .5+
 int8(1/3) gives you 1/3 as an 8 bit integer which is 0, because it rounds down from .333
 -5^2 gives you -25 because without parenthesis, PEMDAS defaults to exponents so 5^2 happens first so we get 25 then times a -1 to get -25 
 (-5)^2 gives you 25 because PEMDAS does parenthesis first, then exponents and so -5 * -5 is a positive 25 
 10 - 6/2 gives you 7 because PEMDAS, so division first then subtraction 
 5*4/2*3 gives you 30 because PEMDAS, and since multiplication and division have the same priority level it goes from left to right 


4 a)

The first example is a = {1,0;2,1} for the variable a which is a 2 x 2 array which has 4 numbers, but each element is individually 8 bytes so there is 8 * 4 = 32 total bytes of data
b is also the same as a, its also a 2 x 2 array
c is a 2 x 1 array
d is either a 1 x 1 array or a 8 byte number 


4 b)

Using the variables from part a, a + b gives a 2 x 2 array adding each element from array a with that of array b so that a + b = [1,0;2,1] + [-1,0;2,1] = [0,0;4,2]

a .* b gives a 2 x 2 array from multiplying each element in the row of the matrix a with each element in the column of matrix b, which is essentially how matrix multiplication works. The final answer is therefore [-1,0;4,1]

a * b  matrix multplication that creates the output.

a * c matrix multiplaction

a + c is adding two arrays of different sizes but it gives the final result as a 2 x 2 array. It adds the first column of a with the only column of c, which becomes the first column of the result, then it adds the second column of a with the only column of c to get the second column for the result which is [4,4; 3,3]

a + d is adding two arrays of different sizes, but because d is just a number it increments each element in the array a by the value d which is 5, so every value in the array a is added by 5 to create the resultant [6,5;7,6]

a .* d is matrix multiplication so the rows of a are multiplied by the columns of d, but since d has only element it would be simply Scalar Multiplication so each element in a is multiplied by d (which is 5) so the result is [5,0;10,5] 

a * d is dot product multiplication or row-wise which is the same as matrix multiplication when dealing with scalars, so the result would still be [5,0;10,5]


5.

a = diag([2,2,2],0) This means the array [2,2,2] should be placed on the major diagonal of a new  3x3 array 

a = 2* eye([3,3]) This means I construct an 3 x 3 identity matrix  and then multiply every value in the matrix by 2. 

a = zeros(3); a(1,1) = 2; a(2,2) = 2; a(3,3) = 2 This essentially generates a 3 x 3 matrix full of zeroes and then the three numbers on the diagonal are changed.


6. 
a1 = 2;   % Variables have to start with a letter 
 b = a1 ; % b is undefined so reversing this sets the value of b to a1 which is 2, and that uses the a1 variable
x = 2;
y = x + 4; % variables are case sensitive
pi = 4 * atan(1); % semicolon disrupted the multiplication
disp(pi);  %semicolon needed to finish disp statement
pi = 3.14159; %pi is used as a number in the next line not as a string
disp(tan(pi));
c = 4^3^2^3;
c = ((c-78564)/c + 32); %have to assign equation to some variable
year = 2017;
disp(['The year is ' , num2str(year)]); % to display 2017 it should convert it to a string with num2str
stuff = {'a' 'b' 4 21 'c'};
beginning = stuff(1); %matlab indices start at 1
End = stuff(5); %end is a keyword
discount = 12; %the percentage sign is used for commentary
AMOUNT = 120.; %subtracting a number from no value doesn't work
amount = 120; %the dollar sign is a key character and shouldn't be used in a numerical value 
class = 'INF1100, gr 2'; %single quotes at both beginning and end
continue_ = x > 0;
fox = false; %comparing a word to boolean value requires usage in a conditional statement, but assigning it to a boolean value is just one equal sign
wolf = fox == true;
Persian = 'Persian is a human language';
Spanish = {'Spanish ' 'is ' ' another'  'language'};
disp(Persian);
disp(Spanish);
disp('Persian is not the same as Spanish');

7. 4 parablolas 
bases at y=0 peaks at y=1
has frequency of pi
