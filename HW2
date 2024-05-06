#include<stdio.h>
#include<stdlib.h>
#include<string.h>
#include<conio.h>

int main()
{
	char ps[5]="2024";
	char en[5];
	int n=1,r,p,m=0;
	char e,t,b;
	char sw;

 printf("程式設計作業\n");
 printf("\n");
    int  i, j, k, l, h;    
    char c = '*';    //ASCII碼里面 3 就是一個字符小愛心 
    
    for (i=1; i<=5; i++)                printf("\n");    //開頭空出5行 
    
    for (i=1; i<=3; i++) 
    {    //前3行中間有空隙分開來寫  
        for (j=1; j<=32-2*i; j++)        
            printf(" ");    //左邊的空格，每下一行左邊的空格比上一行少2個 //8*n-2*i 
        for (k=1; k<=4*i+1; k++)        
            printf("%c", c);//輸出左半部分字符小愛心 
        for (l=1; l<=13-4*i; l++)        
            printf(" ");    
        for (h=1; h<=4*i+1; h++)        
            printf("%c", c);
        printf("\n");        //每一行輸出完畢換行 
    }
    
    for (i=1; i<=3; i++) 
    {    //下3行中間沒有空格 
        for (j=1; j<=24+1; j++)            
            printf(" ");    //左邊的空格 //8*(n-1)+1
        for (k=1; k<=29; k++)            
            printf("%c", c);
        printf("\n");        
    }
    
    for (i=7; i>=1; i--) 
    {    //下7行 
        for (j=1; j<=40-2*i; j++)        
            printf(" ");    //左邊的空格，每下一行左邊的空格比上一行少2個//8*(n+1)-2*i
        for (k=1; k<=4*i-1; k++)        
            printf("%c", c);
        printf("\n");        
    }
    
    for (i=1; i<=39; i++)                
        printf(" ");    
    
    printf("%c\n", c);         
    
    for (i=1; i<=5; i++)                
        printf("\n");  
do{
		printf("請輸入密碼:");
		scanf("%s",en);
		if(strcmp(ps,en)==0){
		break;
		}		
			else if(n==3){
			printf("錯%d次!再見~~~\n",n);
				return 0;
				}
			else{			
			printf("錯%d次!\n",n);
			n++;
			}
				
	}while(n<=3);	

			system("CLS");
			menu:
			puts("---------------------------------");  
			puts("|      a. 畫出n階直角三角形      |");
			puts("|      b. 顯示九九乘法表         |");
			puts("|      c. 結束                   |");
			puts("---------------------------------");
			printf("enter case:");
			fflush(stdin);
			scanf("%c",&sw);
			switch(sw)
			{
				case 'a':
				case 'A':
					system("CLS");
					restart_a:
					printf("Enter char(a~n)\n");
					fflush(stdin);
				    scanf("%c",&e);
				    fflush(stdin);
				    r=e;  //row
				    p=e;  //
				    
					if(e>='a'&&e<='n'){
					for(int i=0;i<=(r-97);i++)
					    {
					        p=i;
					        for(int n=1;n<=(r-97)-i;n++)
					        {
					            printf(" ");
					        }
					        for(int j=0;j<=i;j++)
					        {  
					             printf("%c",e-p);
					            p--;                 
					        }
					        printf("\n");
					    }
					}else{
						printf("輸入錯誤 重新輸入\n");
						goto restart_a;
					}
						system("pause");
						system("CLS");
						goto menu;
				case 'b':
				case 'B':
				restart_b:
					printf("Enter one number(1~9):");	
					scanf("%d",&m);
					if(m>=1&&m<=9){
					for(int a=1;a<=m;a++){
						for(int b=1;b<=m;b++)
						printf("%d*%d=%d ",a,b,a*b);
					printf("\n");
					}
				}else{
					printf("Wrong input,Please enter again\n");
					goto restart_b;
				}
				system("pause");
				system("CLS");
				goto menu;
				case 'c':
				case 'C':
					restart_c:
					printf("Continue?(y/n)");
					fflush(stdin);
					scanf("%c",&c);
					if(c=='y'||c=='Y'){
						system("CLS");
						goto menu;
					}
					if(c=='n' || c=='N'){						
						return 0;
					}else{
						printf("錯誤訊息 請再輸入一次'\n");
						goto restart_c;
					}
				default:
					printf("錯誤輸入\n請再輸入一次\n");
					system("pause");
					system("CLS");
					goto menu;
		}

return 0;	
}
 
