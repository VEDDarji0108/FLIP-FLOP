# FLIP-FLOP
//S-R FLIP FLOP
#include <stdio.h>
#include <stdbool.h>

int main() {
    bool S, R, Q, Q_bar;
    printf("Enter S and R values (0 or 1): ");
    scanf("%d %d", &S, &R);

    // Check for invalid input
    if ((S == 1 && R == 1) || (S == 0 && R == 0)) {
        printf("Invalid input: S and R cannot both be 1 or 0.\n");
        return 1;
    }

    // Implement S-R flip-flop
    if (S == 1 && R == 0) {
        Q = 1;
        Q_bar = 0;
    } else if (S == 0 && R == 1) {
        Q = 0;
        Q_bar = 1;
    } else {
        printf("Invalid input: S and R cannot both be 1 or 0.\n");
        return 1;
    }

    // Output Q and Q_bar values
    printf("Q = %d, Q_bar = %d\n", Q, Q_bar);

    return 0;
}
// J-K FLIP-FLOP 
#include <stdio.h>
typedef char bit;

bit jk(bit J,bit K,bit Q)
{
    return J&~(Q)|Q&~(K);
}

int main()
{
    int i,j,k,a,res=0;
    int x,y,z;
    char b;
    printf("1.Truth Table of JK flip flop");
    printf("\n2.I/O operation\n");
    printf("Enter your choice: ");
    scanf("%d",&a);
    
    switch(a) 
    {
        case 1:
            printf("J  K  Q(t) | Q(t+1)\n");
            for(i=0;i<2;i++)
            {
                for(j=0;j<2;j++)
                {
                    for(k=0;k<2;k++)
                    {
                        res=jk(i,j,k);
                        printf("%d  %d  %d    |",i,j,k);
                        printf("  %d\n",res);
   
                    }
                }
            }
            break;
  
        case 2:
            printf("Enter the value of J,K,Q(t):");
            scanf("%d%d%d",&x,&y,&z);
 
            res=jk(x,y,z);
            printf("Q(t+1)= %d\n\n",res);

            break;

        default:
            printf("invalid input");   
         
    }
    printf("do you want to continue(Y/N):");
    scanf(" %c",&b);
    if(b=='Y'||b=='y')
    {
        main();
    }
    else
    {
        return 0;
    }
}

