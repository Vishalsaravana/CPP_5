# STACK APPLICATIONS
## PROGRAM STATEMENT :

To write a CPP program for Infix to Postfix Conversion using Stack STL

## ALGORITHM:  

1.	Define a function priority to assign precedence to operators.
2.	Create a postfix string and a stack to hold operators.
3.	Loop through each character in the infix expression, processing operands and operators.
4.	Handle parentheses by pushing and popping from the stack.
5.	After processing the expression, pop any remaining operators from the stack to postfix.
6.	Print the resulting postfix expression.
7.	End the program

## PROGRAM:
```
// Usinginbuilt stack libraryto createstack #include <iostream>
#include <stack> #include <string> usingnamespacestd;

int priority (char alpha){ if(alpha == '+' ||alpha =='-')
return 1;

if(alpha == '*' || alpha=='/') return 2;

if(alpha == '^') return 3;

return 0;
}
string convert(string infix)
{
int i= 0;
stringpostfix = "";
// using inbuilt stack<> from C++stacklibrary

stack<int> s;
 
while(infix[i]!='\0')
{
// ifoperand add to thepostfix expression
if( ( (infix[i]>='a') && (infix[i]<='z') ) || ( (infix[i]>='A') && (infix[i]<='Z')) )
{
postfix+= infix[i]; i++;
}
// ifopening bracket thenpushthestack else if(infix[i]=='(')
{
s.push(infix[i]); i++;
}
// if closing bracket encounted thenkeep popping fromstack until
// closingapairopeningbracket is not encountered else if(infix[i]==')')
{
while(s.top()!='('){ postfix += s.top(); s.pop();
}
s.pop(); i++;
}
else
{
while(!s.empty() && priority(infix[i]) <= priority(s.top())){ postfix += s.top();
s.pop();
}
s.push(infix[i]); i++;
}
}
while(!s.empty()){ postfix += s.top(); s.pop();
}


cout << "Postfix is : " << postfix;//it willprint postfixconversion return postfix;
}

int main()
{
string infix;
 
string postfix; cin>>infix;
postfix == convert(infix);

return 0;
}
```

## OUTPUT :
![image](https://github.com/user-attachments/assets/a104b42f-7bb8-4b91-83f8-b17ea7ccd885)


## RESULT :

Thus, the C++ program for Infix to Postfix Conversion using Stack STL is created successfully.
 

