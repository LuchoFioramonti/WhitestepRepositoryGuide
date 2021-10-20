# WhitestepRepositoryGuide

#include <stdio.h>
#include <stdlib.h>

int main(int argc, char *argv[])
{
  float vector1[10], vector2[10], vector3[10]; // declaro los arrays
  float mayornumv1; // variable mayor num vector 1
  float promediov2; // variable promedio vector 2
  int i=0; // contador1
  int n=0; // suma vector2
  
  for (i=0; i<10; i++)
    {
        vector1[i] = 5;
        if (vector1[i] > mayornumv1)
        mayornumv1 = vector1[i];
    }
  i = 0;
  
  for (i=0; i<10; i++)
    {
        printf("INGRESE EL VALOR DE LA POSICION %d\n", i+1);
        scanf("%f", &vector2[i]);
        n = vector2[i];
        promediov2 = n+promediov2;
    }
  i = 0;  
  printf("EL PROMEDIO DEL VECTOR2 ES: %.2f\n", promediov2/10);
  
  printf("LA SUMA DEL CUARTO ELEMENTO DE VECTOR1 Y EL OCTAVO ELEMENTO DE VECTOR2 ES: %.2f\n", vector1[3]+vector2[7]);
  
  for (i=0; i<10; i++)
    {
        vector3[i] = vector2[i]*3;
    }
  i = 0;
  
  printf("VECTOR 1 / VECTOR 2 / VECTOR 3\n");
  for (i=0;i<10;i++)
    {
        printf("\n%.2f", vector1[i]);
        printf("      %.2f", vector2[i]);
        printf("         %.2f", vector3[i]);
        
    }  
  printf("\nEL PROGRAMA HA FINALIZADO\n");
  
  system("PAUSE");	
  return 0;
}
