# EXPT.NO.9-IMPLEMENTATION-OF-GO-BACK-N-PROTOCOL-SELECTIVE-REPEAT
# AIM:
To write and execute a program for Go-Back-N protocol-Selective Repeat.
# EQUIPMENTS REQUIRED:
Personal Computer Turbo C Compiler
# PROCEDURE:
**STEP 1:** Connect two computers in Wired/Wireless LAN.
**STEP 2:** Make sure that two computers are in one network and could able to ping each other.
**STEP 3:** In the codeblocker open new c file and type the program.
**STEP 4:** In the menu choose->Project->Properties->Project Build options->Linker settings->Add netproto and pthread.
**STEP 5:** Execute the program in both server and client.
**STEP 6:** Enter the IP address of the remote machine, port address of both local & remote machine and error rate.
**STEP 7:** Choose the file and verify the go back protocol oper

# PROGRAM:
```
#include<stdio.h> void main()
{

int i,j,n;
printf("GO BACK N ARQ\n");
//printf("Entermessage in format\n"); printf("Enter number of frame : "); scanf("%d",&n);
char frame[n][10];

for(i=1;i<=n;i++)
{
printf("Content for frame %d :",i); scanf("%s",&frame[i]);
}
int s=1;
//while(j<=n){
printf("Enter frame number with no ACK :"); scanf("%d",&j);
for(i=1;i<=n;i++)
{
if(i!=j)
printf("\n Sending frame %d \n FRAME ACKNOWLEDGED.	\n",i);
//else
//printf("\n Frame not Acknowledeged.	\n");
 
}
if(j<=n)
{
printf("No Acknowlegement for frame %d... \n",j); printf("Resending... Content from frame %d :%s\n\n",j,frame[j]);

}
printf("\n Sending frame %d \n FRAME ACKNOWLEDGED.	\n",j);
//}

printf("\n\nALL FRAME RECIEVED SUCCESSFULLY\n\n");
}
```
# OUTPUT:

 <img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/11466840-7be8-4562-b685-319c84d05465" />

# RESULT:
Thus the Go-Back-N protocol- Selective Repeat was implemented and the output is verified successfully.
