#include <stdio.h>
int main(){
    int a ,b;
    scanf("%d" ,&a);
    b = 2;
    while(a > 1){
        if(a % b == 0){
            printf("%d\n" ,b);
            a = a/b;
        }
    }
    return 0;
}# zerojudge
