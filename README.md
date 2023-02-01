# Linguagem-C
Projetos iniciais
#include <stdio.h>
#include <stdlib.h>
#include <string.h>


int main(){
char nome[100], alf[] = {'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z'};
int a, b, cont = 0;
gets(nome);
for(a = 0; alf[a]; a++){

        for(b = 0; nome[b]; b++ ){
          if(nome[b] == alf[a]){
            printf("[%c]", nome[b]);
            cont = cont + 1;
            }
        }
    if(cont >= 1){
        printf(" a palavra (%s) tem (%d) letras (%c) \n", nome, cont, alf[a]);
        cont = 0;
    }
}

}
