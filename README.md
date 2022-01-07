#include <stdio.h>
#include <math.h>

int main(void) {
  float a,b,c, delta, x1, x2;

  printf("A: ");
    scanf("%f", &a);

  printf("B: ");
    scanf("%f", &b);

  printf("C: ");
    scanf("%f", &c);
   
  delta = (b*b) - (4*a*c);
  
  printf("\nDelta: %.2f", delta);



  if(a!= 0){
    delta =(b*b) - 4*a*c;
    if (delta ==0){
      x1 = (-b + sqrt(delta)) / (2*a);
      printf("Delta = 0");
      printf("X1= %.2f", x1);
      printf("X2= %.2f", x1);
    }
  }
  
  if(delta < 0){
    printf("Não é possível resolver raizes negativas!");
  }
  else{
    if(delta > 0){
    x1 = (-b + sqrt(delta)) / (2 * a);
    x2 = (-b - sqrt(delta)) / (2 * a);
    
    printf("\n\nX1 = %.2f", x1);
    printf("\nX2 = %.2f", x2);
    }
  }
  return 0;
}
