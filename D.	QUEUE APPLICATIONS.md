# QUEUE APPLICATIONS

## PROGRAM STATEMENT :

To write a C++ program to implement FCFS algorithm(no of process p1,p2 and p3 and its burst time are 10,5 & 8) find out waiting time of the each process & Average waiting time of the process.

## ALGORITHM:  

1.	Start the program.
2.	Define findWaitingTime to take process IDs, count of processes n, and burst times bt.
3.	Initialize wt for waiting times and set wt[0] = 0.
4.	Use a loop to calculate each waiting time as wt[i] = bt[i-1] + wt[i-1].
5.	Print "Processes", "BT time", and "WT time" table headings.
6.	Use a loop to print each process's ID, burst time, and waiting time, adding each to total_wt.
7.	Print average waiting time as total_wt / n.
8.	In main, define processes, n, and bt, then call findWaitingTime.
9.	End the program.

## PROGRAM:
```
#include<iostream> using namespace std;
void findWaitingTime(int processes[], int n,int bt[])
{
intwt[n];
float total_wt=0;
// waitingtimefor first process is 0 wt[0]=0;
// calculatingwaitingtime for (int i= 1; i< n ; i++ )
wt[i] = bt[i-1] +wt[i-1] ;

cout << "Processes "<<" BT time "<< " WT time \n"; for (int i=0; i<n; i++)
{
total_wt =total_wt + wt[i];
cout << "	" << i+1 << "	" << bt[i] <<"	"<<wt[i]<<endl;
}

cout<<"Averagewaitingtime="<<total_wt/n<<endl;
}
 
// Driver code int main()
{
//process id's
int processes[]={1,2,3}; int n = 3;

int bt[]={10,5,8};

findWaitingTime(processes, n, bt); return 0;
}
```

## OUTPUT :
![image](https://github.com/user-attachments/assets/71695c0e-9b9b-4796-9531-cff2ffc6ffee)

## RESULT :

Thus, the C++ program to implement FCFS algorithm(no of process p1,p2 and p3 and its burst time are 10,5 & 8) find out waiting time of the each process & Average waiting time of the process ADT is created successfully.

