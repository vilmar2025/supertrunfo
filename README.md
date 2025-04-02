
#include <stdio.h>

typedef struct {
    char nome[50];
    int atributo;
} Carta;

int main() {
    Carta carta1, carta2;

    // Dados das cartas (exemplo)
    printf("Digite o nome da Carta 1: ");
    scanf("%s", carta1.nome);
    printf("Digite o valor do atributo da Carta 1: ");
    scanf("%d", &carta1.atributo);

    printf("Digite o nome da Carta 2: ");
    scanf("%s", carta2.nome);
    printf("Digite o valor do atributo da Carta 2: ");
    scanf("%d", &carta2.atributo);

    // Comparação
    if (carta1.atributo > carta2.atributo) {
        printf("%s vence!\n", carta1.nome);
    } else if (carta2.atributo > carta1.atributo) {
        printf("%s vence!\n", carta2.nome);
    } else {
        printf("Empate!\n");
    }

    return 0;
}