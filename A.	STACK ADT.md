# STACK ADT
## PROGRAM STATEMENT :

To Write a CPP Program to insert five character elements in to Stack ADT (use STL for Stack.

## ALGORITHM:  

1.	Start the program.
2.	Initialize a stack of characters named mystack.
3.	Read an integer n as the size of the stack.
4.	Print the size of the stack.
5.	Use a loop to read n characters and push each character onto the stack.
6.	Use a loop to pop and print each character from the stack until the stack is empty.
7.	End the program.

## PROGRAM:
```
#include<iostream> #include<stack> usingnamespacestd; int main()
{
stack<char>mystack; int n,i;
char c; cin>>n;
cout<<"Size ofthestack: "<<n<<endl; for(i=0;i<n;i++){
cin>>c; mystack.push(c);
}
while(!mystack.empty()){ cout<<mystack.top()<<" "; mystack.pop();
}
}
```
## OUTPUT :
![image](https://github.com/user-attachments/assets/5ae50aba-6ee0-426c-aa1f-5cd55931aebc)


## RESULT :
Thus, the C++ program to insert five character elements in to Stack ADT is created successfully.
 
