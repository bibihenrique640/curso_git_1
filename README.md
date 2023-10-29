# curso_git_1
#include <stdio.h>

float soma(float n1, float n2){
    return n1 + n2;
}

float subtracao(float n1, float n2){
    return n1 - n2;
}

float multiplicacao(float n1, float n2){
    return n1 * n2;
}

float divisao(float n1, float n2){
    return n1 / n2;
}


int main(){
    char resposta_se_quer_continuar;
    int numero1;
    int numero2;
    int escolha;
    do{
        printf("Digite o primeiro e o segundo numero: ");
        scanf("%d" "%d", &numero1, &numero2);

        printf("Escolha: 1- somar\n2- subtrair\n3- multiplicar\n4- dividir");
        scanf("%d", &escolha);
        switch(escolha){
            case 1:
            printf("A soma de %d e %d eh: %f", numero1, numero2, soma(numero1, numero2));
            break;

            case 2:
            printf("A subtracao de %d e %d eh: %f", numero1, numero2, subtracao(numero1, numero2));
            break;

            case 3:
            printf("A multiplicacao de %d e %d eh: %f", numero1, numero2, multiplicacao(numero1, numero2));
            break;

            case 4:
            printf("A divisao de %d e %d eh: %f", numero1, numero2, divisao(numero1, numero2));
            break;

            default:
            printf("Opcao invalida.\n");
            break;
        }

        printf("Deseja fazer outra operacao (s/n)");
        scanf(" %c", &resposta_se_quer_continuar);

    }while(resposta_se_quer_continuar == 's');

    printf("TMJ YODAO");


}
