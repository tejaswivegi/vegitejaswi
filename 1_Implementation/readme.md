#include //header file
#include //header file
#include //header file
#include //header file
#include //header file
void main()
{
clrscr();

//declartion of variables that are required in the program

char name[20],date[40],ch1='y',ch2='y',pro[100];
float rate,cost=0.0,total=0.0,c[100];
int bill,sno=0,quantity,q[100],product,i;
FILE *fp; //creating a file with pointer named fp
fp=fopen("store.c","r"); //opening the file named store.c

//inputting the variables using odd for loop

while(ch1=='y')
{
printf("ENTER COUSTOMER'S NAME ");
scanf("%s",&name);
printf("\nENTER BILL NUMBER ");
scanf("%d",&bill);
printf("\nENTER DATE ");
scanf("%s",&date);
printf("\nENTER NAME OF THE PRODUCT ");
printf("\nPLEASE\nPRESS 1 FOR SOAP \nPRESS 2 FOR BRUSH \nPRESS 3 FOR PASTE \nPRESS 4 FOR RING \nPRESS 5 FOR NOTE BOOK\n ");
ch2='y';

//entering the quantities required by the coustomer using odd while loop

while(ch2=='y')
{
printf("\nENTER YOUR CHOICE ");
scanf("%d",&product);

//switch case to know the product bought by the coustomer

switch(product)
{

//case to calculate cost quantity and total

case 1:
printf("\nENTER QUANTITY ");
scanf("%d",&quantity);
rate=20;
cost=quantity*20;
sno++;
c[sno]=cost;
total=total+cost;
pro[sno]=product;
q[sno]=quantity;
break;

//case to calculate cost quantity and total

case 2:
printf("\nENTER QUANTITY");
scanf("%d",&quantity);
rate=5;
sno++;
cost=quantity*5;
c[sno]=cost;
total=total+cost;
pro[sno]=product;
q[sno]=quantity;
break;

//case to calculate cost quantity and total

case 3:
printf("\nENTER QUANTITY");
scanf("%d",&quantity);
rate=30;
sno++;
cost=quantity*30;
c[sno]=cost;
total=total+cost;
pro[sno]=product;
q[sno]=quantity;
c[sno]=cost;
break;

//case to calculate cost quantity and total

case 4:
printf("\nENTER QUANTITY");
scanf("%d",&quantity);
rate=10;
sno++;
cost=quantity*10;
c[sno]=cost;
total=total+cost;
pro[sno]=product;
q[sno]=quantity;
break;

//case to calculate cost quantity and total

case 5:
printf("\nENTER QUANTITY");
scanf("%d",&quantity);
rate=15;
sno++;
cost=quantity*15;
c[sno]=cost;
total=total+cost;
pro[sno]=product;
q[sno]=quantity;
break;
default:
printf("\nINVALID RESPONSE");
} //end of switch
printf(" \nANY MORE PRODUCT PRESS 'y' AND 'n' FOR NO");
fflush(stdin);
scanf("%c",&ch2);
}

//end of while loop

fclose(fp);

//close of file store.c
//opening hte file store.c in append mode

fp=fopen("store.c","app");
//to displat the deatils of coustomer

printf("\nCOUSTOMER'S NAME:%s",name);
printf("\tBILL NO.%d",bill);
printf("\nDATE%s",date);

//to display the products bought by them

printf("\nS NO.\tPRODUCT\tRATE\tQUANTITY\tCOST");
for(i=1;i<=sno;i++) //for loop begins to display the details
{
printf("\n%d",i);
if(pro[i]==1)
{
printf("\tSOAP\t");
printf("20");
}
else if(pro[i]==2)
{
printf("\tBRUSH\t");
printf("5");
}
else if(pro[i]==3)
{
printf("\tPASTE\t");
printf("30");
}
else if(pro[i]==4)
{
printf("\tRING\t");
printf("10");
}
else
{
printf("\tNOTEBOOK");
printf("15");
}
printf("\t%d",q[i]);
printf("\t\t%f",c[i]);
printf("\n");
}

//end of for loop

printf("\nTOTAL%f",total); //to displat the total
printf("\n");

//to know whether there is next coustomer and to input their details

printf("\nNEXT CUSTOMER");
printf("\nPRESS 'y' TO CONTINUE ");
fflush(stdin);
scanf("%c",&ch1);

//for loop to intailise all the variables to zero

for(i=1;i<=sno;i++)
{
pro[i]=0;
q[i]=0;
c[i]=0;
}

//end of for loop

}

//end of while loop

cost=0,total=0,quantity=0;
fclose(fp);

//close of file
getch();
}
//close of main
//close of program
