# quadequation1vari
#include <stdio.h>
#include <stdlib.h>
#include <math.h>

int main()
{
    float a,b,c,d,x1,x2; //d: discriminant

    printf("WELCOME\nTo find the roots of a quadratic equation with one variable,");
    printf("\n\nEnter the coefficient for x^2:");
    scanf("%f",&a);

    printf("\nEnter the coefficient for x:");
    scanf("%f",&b);

    printf("\nEnter the constant term:");
    scanf("%f",&c);

    printf("\nEquation is:(%dx^2)+(%dx)+(%d)=0\n",(int)a,(int)b,(int)c);

    d=b*b-(4*a*c);

    if(d<0)
   {
   printf("\nRoots are imaginary.\n");
   return 0;
   }

      else if(d==0)
      {
      x1=-b+sqrt(d)/2*a;
      printf("\nThere is a single root for this equation.\nThe root is: %f\n",x1);
      return 0;
      }

         else if(d>0);
         {

         x1= (-b+sqrt(d))/2*a;
         x2= (-b-sqrt(d))/2*a;

         printf("\nRoot1= %f",x1);
         printf("\nRoot2= %f\n",x2);
         }
    return 0;
}
