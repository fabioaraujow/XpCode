#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include <conio.h>
void limpar_entrada() {
char c;
while ((c = getchar()) != '\n' && c != EOF) {}
}
int main()
{
    int i, rato, sapo, coelho, ret, totalC;
    double  N, Q, pCoelhos, pRatos, pSapos;
    char tipoC, c;

    printf("Informe quantos casos serao digitados: ");
    ret = scanf("%lf", &N);

    while (ret == 0 || N != (int)N || N < 0)
    {
        printf("Dado(s) Invalido(s). Tente novamente!: ");
        limpar_entrada();
        ret = scanf("%lf", &N);
    }

    rato = 0;
    coelho = 0;
    sapo = 0;

    for (i = 0; i < N; i++)
    {
        printf("Quantidade de cobaias: ");
        ret = scanf("%lf", &Q);

        while (ret == 0 || Q != (int)Q || Q < 0)
        {
            limpar_entrada();
            printf("Dado(s) Invalido(s). Tente novamente!: ");
            ret = scanf("%lf", &Q);
        }

        printf("Tipo de Cobaia: ");
        limpar_entrada();
        scanf("%c", &tipoC);
        while (tipoC != 'R' && tipoC != 'S' && tipoC != 'C' && tipoC != 'r' && tipoC != 's' && tipoC != 'c')
        {
            printf("Dado(s) invalidos! Tente novamente: ");
            limpar_entrada();
            scanf("%c", &tipoC);
        }
        if (tipoC == 'R' || tipoC == 'r')
        {
            rato = rato + Q;
        }
        else if (tipoC == 'C' || tipoC == 'c')
        {
            coelho = coelho + Q;
        }
        else if (tipoC == 'S' || tipoC == 's')
        {
            sapo = sapo + Q;
        }
    }
        printf("Relatorio Final:\n");
        totalC = rato + coelho + sapo;
        printf("Total de Cobaias: %d cobaias.\n", totalC);
        printf("total de Coelhos: %d\n", coelho);
        printf("total de Ratos: %d\n", rato);
        printf("total de Sapos: %d\n", sapo);
        pCoelhos = (double)(coelho * 100)/(double)totalC;
        printf("Percentual de coelhos: %.2lf\n", pCoelhos);
        pRatos = (double)(rato * 100)/(double)totalC;
        printf("Percentual de ratos: %.2lf\n", pRatos);
        pSapos = (double)(sapo * 100)/(double)totalC;
        printf("Percentual de sapos: %.2lf\n", pSapos);
        printf("\n");

    return 0;
}
