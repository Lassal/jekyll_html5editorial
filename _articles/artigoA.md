---
 layout: article
 title: Meu artigo de teste
 head_image: https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Elizabeth_Quay_February_2016_%28cropped%29.jpg/1200px-Elizabeth_Quay_February_2016_%28cropped%29.jpg
---

Meu titulo principal
-------------------------------------------------------

Todas estas questões, devidamente ponderadas, levantam dúvidas sobre se o consenso sobre a necessidade de qualificação desafia a capacidade de equalização das direções preferenciais no sentido do progresso.
O empenho em analisar o desenvolvimento contínuo de distintas formas de atuação maximiza as possibilidades por conta dos métodos utilizados na avaliação de resultados.
No entanto, não podemos esquecer que o aumento do diálogo entre os diferentes setores produtivos nos obriga à análise do levantamento das variáveis envolvidas.

A Ana Rosa disse que era um lero lero *<=oD

**O Gustavo e muito louco ha ha ha**

---------------------------

No entanto, não podemos esquecer que a determinação clara de objetivos apresenta tendências no sentido de aprovar a manutenção dos conhecimentos estratégicos para atingir a excelência.


---------------------------------
## Um exemplo de código
Abaixo temos um exemplo de implementação de pilha em linguagem C.


```c
#include <stdio.h>

int MAXSIZE = 8;       
int stack[8];     
int top = -1;            

int isempty() {

   if(top == -1)
      return 1;
   else
      return 0;
}

int isfull() {

   if(top == MAXSIZE)
      return 1;
   else
      return 0;
}

int peek() {
   return stack[top];
}

int pop() {
   int data;

   if(!isempty()) {
      data = stack[top];
      top = top - 1;   
      return data;
   } else {
      printf("Could not retrieve data, Stack is empty.\n");
   }
}

int push(int data) {

   if(!isfull()) {
      top = top + 1;   
      stack[top] = data;
   } else {
      printf("Could not insert data, Stack is full.\n");
   }
}

int main() {
   // push items on to the stack
   push(3);
   push(5);
   push(9);
   push(1);
   push(12);
   push(15);

   printf("Element at top of the stack: %d\n" ,peek());
   printf("Elements: \n");

   // print stack data
   while(!isempty()) {
      int data = pop();
      printf("%d\n",data);
   }

   printf("Stack full: %s\n" , isfull()?"true":"false");
   printf("Stack empty: %s\n" , isempty()?"true":"false");

   return 0;
}
```
