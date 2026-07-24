#include <stdio.h>
int main(){
    int a ,b ,c ,d;
    scanf("%d" ,&a);
    b = 2;
    c = 0;
    d = 0; 
    while(a > 1){
        if(a % b == 0){
            a = a/b;
            c = c+1;
            if (a%b != 0){
                printf("%d%c%d ",b ,'^' ,c);
                c = 0;
            }
            if (d > 0){
                printf("%c " ,'*');
                d = 0;
            }
        }
        else{
            b = b+1;
            d +=1;
        }
    }
    return 0;
}
