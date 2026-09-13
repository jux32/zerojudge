#include <stdio.h>
int main(){
    int a[3][2] = {{1 ,2} ,{3 , 4} , {5, 6}} ;
    int b[2][3] ,x ,y ,i;
    x = 0;
    y = 0;
    i = 0;
    while (i <= 5){//執行6次
        printf ("i = %d\n" ,i);
        if (x <= 1){
            printf( "x = %d\n" , x);
            printf( "y = %d\n" , y);
            x += 1;
        }
        else if (x == 2 & y <= 3){
            printf( "y = %d\n" , y);
            printf( "x = %d\n" , x);
            y += 1;
        }
        else{

        }
        i += 1;

    }
    return 0;
}
