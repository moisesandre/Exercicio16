# Exercicio16

#include <stdlib.h>
#include <stdio.h>
#include <string.h>
#include <ctype.h>
main ()
{

    char frase[50];
    int i, tam;

    printf("Digite uma frase: \n");
    gets(frase);

    tam = strlen(frase);

    for (i=0; i<tam; i++)
    {
        switch (tolower(frase[i]))
        {
        case 'a':
            frase[i]='x';
            break;
        case 'e':
            frase[i]='y';
            break;
        case 'i':
            frase[i]='w';
            break;
        case 'o':
            frase[i]='k';
            break;
        case 'u':
            frase[i]='z';
            break;
        }
    }

    system("cls");
    printf("Frase criptografada\n%s\n",frase);

    return 0;
}
