#include <stdio.h>
int main(){
   int number ,a ,power;
   a = 2;  // 除數
   power = 0; // 指數
   scanf("%d" ,&number);
   while (number > 1 ){
      if (number % a != 0){
         a += 1;
         power = 0;
      }
      if (number % a == 0){
         number = number / a;
         power += 1;
      }
      if (power > 1 & number % a != 0){
         printf("%d^%d" ,a ,power);
         if (number > 1){
            printf(" * ");
         }
      }
      if (power == 1 & number % a != 0){
         printf("%d" ,a);
         if (number > 1){
            printf(" * ");
         }
      }
   }
   return 0;
}
