#include <stdio.h>
int main(){
    int a[3][2] = {{1 ,2} ,{3 , 4} , {5, 6}} ;
    int b[2][3] ,x ,y ,i;
    x = 0;
    y = 0;
    i = 0;
    while (x <= 1){
        while (y <= 2){
            b[x][y] = a[y][x];
            printf("b[%d][%d]%d " , x, y,b[x][y]);
            y += 1;
        }
        printf ("\n");
        x += 1;
        y = 0;
    }

    return 0;
}
