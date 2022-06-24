# CodeChallenge

Question: 

Function SystemOfEquations will receive a string str Which will be a list of equations. The system of equations will consist of an unspecified number of equations formatted like:

varname = [ number1 | varname1 ] { ^ [ number2 | varname2 ] } { ^ [ number3 | varname3 ] } ...

Where:
varname is made up of letters. Example: a, ke, ikall
number is a integer number
^ represents the operator XOR (Exclusive OR). XOR operator is a bitwise operator that compares the bits one by one and returns 0 if the matching bits are the same and returns 1 if the matching bits are different (not the same)

Each equation represents an assignment (=) that sets a value to the var varname. The list of equations will be passed as a String whose equations are separated by a semi-colon and a blank (‘; ‘). In addition, the following assumptions can be made:

The same var cannot be on the left side of multiple equations, just on one or none. The equations do not follow any particular order. Your function must find the value of the variable “x”. When the solution is impossible to be reached, the function will return the string null.

Your function must find the value of the variable “x”. When the solution is impossible to be reached, the function will return null.

# Sample Test Cases:

1. For input "z = p ^ p ^ 2430 ^ 3231 ^ 1904; p = 8902 ^ 1521 ^ a ^ 8369; r = a ^ a ^ 5426 ^ z ^ z ^ a ^ a ^ 6023 ^ z ^ p; a = 3282; x = p ^ p ^ p ^ z ^ p ^ a ^ z ^ a ^ r ^ a" the output was incorrect. The correct output is 1954

2. For input "v = 1021 ^ s ^ 6219 ^ f ^ t ^ 4253 ^ 6048 ^ u ^ t ^ f; u = s ^ 6760 ^ 6437 ^ r ^ s ^ r ^ r ^ s ^ 3693 ^ r; s = r ^ 491 ^ 8958 ^ 2691 ^ 2301 ^ r ^ 4161 ^ r ^ r ^ r; t = r ^ 1857 ^ 8277; l = u ^ g ^ f ^ 3321 ^ 2379 ^ 450 ^ w ^ 3863 ^ r ^ u ^ 5220; h = 4239 ^ u ^ 2275; n = 9869 ^ 1548 ^ s ^ r ^ 6741 ^ g ^ 6294 ^ t; r = 6064 ^ 7882 ^ 3937 ^ 6882 ^ 8888 ^ 7797 ^ 5094 ^ 1362; g = w ^ s; x = v ^ r ^ w ^ h ^ v ^ v ^ s ^ s ^ n ^ n ^ r ^ l; w = 9659 ^ 8764 ^ 9106 ^ v ^ 2181 ^ 6558; f = 9483 ^ u" the output was incorrect. The correct output is 9792
