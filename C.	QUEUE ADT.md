# QUEUE ADT
## PROGRAM STATEMENT :

To write a CPP Program to insert 5 operator elements in to Queue ADT.

## ALGORITHM:  

1.	Create a queue of characters using queue<char>.
2.	Input 5 characters using a loop and push each character into the queue.
3.	Print the message "Queue Elements are:".
4.	Use a while loop to traverse the queue until it is empty.
5.	For each iteration, print the front element of the queue using que.front().
6.	Remove the front element from the queue using que.pop()
7.	End the program

## PROGRAM:
```
#include <iostream> #include <queue> usingnamespacestd; int main()
{
queue<char>que; char c;
for(int i=0;i<5;i++)
{
cin>>c; que.push(c);
}
cout<<"QueueElementsare:"; while(!que.empty())
{
cout<<que.front()<<" "; que.pop();
}
}
```
## OUTPUT :
![image](https://github.com/user-attachments/assets/345bedac-62ca-4e51-90fa-d1f5293d0d2a)

## RESULT :

Thus, the C++ program to insert 5 operator elements in to Queue ADT is created successfully.
 


