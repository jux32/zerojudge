#include <stdio.h>
int main(){
    int x ,y ,xi ,yi;
    scanf ("%d %d",&x ,&y);//x乘y 矩陣
    int a[x][y] ,b[y][x];//儲存盒

    for (int i = 0; i < x; i++){
        for (int j = 0; j < y; j++){
            scanf("%d", &a[i][j]);   
        }
    }
    xi = 0;
    yi = 0;
    while (yi <= (y-1)){
        while (xi <= (x-1)){
            b[yi][xi] = a[xi][yi];
            printf("b[%d][%d]%d " , yi, xi,b[yi][xi]);
            xi += 1;
        }
        printf ("\n");
        yi += 1;
        xi = 0;
    }
    return 0;
}
