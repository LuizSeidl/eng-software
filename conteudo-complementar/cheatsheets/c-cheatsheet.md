# 📋 C Cheatsheet

## Estrutura básica
#include <stdio.h>

int main() {
  printf("Olá Mundo\n");
  return 0;
}

## Tipos de dados
int x = 10;
float y = 3.14;
double z = 3.14159;
char c = 'A';
char s[] = "texto";

## Entrada e saída
printf("Valor: %d\n", x);   # imprime
scanf("%d", &x);             # lê

## Formatadores
%d    # inteiro
%f    # float
%lf   # double
%c    # char
%s    # string

## Operadores
+  -  *  /  %     # aritméticos
==  !=  >  <  >=  <=  # comparação
&&  ||  !          # lógicos

## Controle de fluxo
if (x > 0) {}
else if (x == 0) {}
else {}

for (int i = 0; i < 10; i++) {}
while (x > 0) {}
do { } while (x > 0);

switch (x) {
  case 1: break;
  default: break;
}

## Funções
int soma(int a, int b) {
  return a + b;
}

## Arrays
int arr[5] = {1, 2, 3, 4, 5};
arr[0]        # acessa elemento

## Ponteiros
int *p = &x;  # ponteiro para x
*p            # valor apontado
p             # endereço

## Structs
struct Pessoa {
  char nome[50];
  int idade;
};

## Alocação Dinâmica (requer <stdlib.h>)
int *ptr = malloc(sizeof(int) * 5);  # aloca espaço para 5 inteiros
free(ptr);                           # libera a memória alocada

## Tamanho de tipos
sizeof(int)                          # retorna o tamanho em bytes