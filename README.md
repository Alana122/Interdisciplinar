#include <stdio.h>
#include <stdlib.h>
#include <string.h>

int main() {
    char mat[5][2][20];
    int i = 0;
    int j = 0;

    strcpy(mat[0][0], "conversa");
    strcpy(mat[1][0], "debate");
    strcpy(mat[2][0], "discussao");
    strcpy(mat[3][0], "troca");
    strcpy(mat[4][0], "interacao");

    strcpy(mat[0][1], "colaboracao");
    strcpy(mat[1][1], "comunicacao");
    strcpy(mat[2][1], "negociacao");
    strcpy(mat[3][1], "argumentacao");
    strcpy(mat[4][1], "entendimento");

    printf("Matriz (ordem inicial):\n");
   
    i = 0;
while (i < 5) {
    j = 0;
    while (j < 2) {
        printf("%-15s", mat[i][j]);
        j++;
    }
    printf("\n");
    i++;
}
printf("\nConteudo do vetor:\n");
    for (i = 0; i < 5; i++) {
        for (j = 0; j < 2; j++) {
            printf("%-15s", mat[i][j]);
        }
    }
   
    printf("\n");
    return 0;
}
