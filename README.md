# Ciclos-y-arreglos-1
ESTE ES EL PRIMER CODIGO DE "CICLOS Y ARREGLOS":

#include <stdio.h>


float calcBmi(float h,float w);


int main(){

    int personas;

    float height;
    float weight;
    float bmi;



    printf("digite el numero de personas: ");
    scanf("%i",&personas);


    for (int contador=0; contador < personas; contador++){
        printf("PERSON %i.\n", contador + 1);
        printf("Enter your height in cms: ");
        scanf("%f",&height);
        printf("Enter your weight in kgs: ");
        scanf("%f",&weight);

        bmi=calcBmi(height,weight);


        printf("Your body mass index is %f kg/m^2\n",bmi);
    }

    }
    
float calcBmi(float h,float w){
    float bmi;


    bmi=w/((h/100.0)*(h/100.0));
    return bmi;
}
