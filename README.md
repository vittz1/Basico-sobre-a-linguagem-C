# Introdução à linguagem C

C é uma linguagem de programação procedural. Foi inicialmente desenvolvido por Dennis Ritchie no ano de 1972. Foi desenvolvido principalmente como uma linguagem de programação de sistema para escrever um sistema operacional. Os principais recursos da linguagem C incluem acesso de baixo nível à memória, um conjunto simples de palavras-chave e um estilo limpo. Esses recursos tornam a linguagem C adequada para programações de sistema, como um sistema operacional ou desenvolvimento de compilador.
Muitas linguagens posteriores emprestaram sintaxe / recursos direta ou indiretamente da linguagem C. Como a sintaxe de Java, PHP, JavaScript e muitas outras linguagens são baseadas principalmente na linguagem C. C ++ é quase um superconjunto da linguagem C (poucos programas podem ser compilados em C, mas não em C ++).

# Começando com a programação C:

Estrutura de um programa C
Após a discussão acima, podemos avaliar formalmente a estrutura de um programa C. Por estrutura, significa que qualquer programa pode ser escrito apenas nesta estrutura. Escrever um programa C em qualquer outra estrutura levará, portanto, a um Erro de Compilação.
A estrutura de um programa C é a seguinte:

![alt text](https://www.codingame.com/servlet/fileservlet?id=38806561194619)

1 - Os componentes da estrutura acima são:

1. **Inclusão de arquivos de cabeçalho**: O primeiro e mais importante componente é a inclusão dos arquivos de cabeçalho em um programa C.
Um arquivo de cabeçalho é um arquivo com extensão .h que contém declarações de funções C e definições de macro a serem compartilhadas entre vários arquivos de origem.

Alguns dos arquivos de cabeçalho C :
* stddef.h - Define vários tipos e macros úteis.
* stdint.h - Define tipos inteiros de largura exata.
* stdio.h - Define funções básicas de entrada e saída
* stdlib.h - Define funções de conversão numérica, gerador de rede pseudo-aleatório, alocação de memória
* string.h - Define funções de manipulação de string
* math.h - Define funções matemáticas comuns

2. Declaração do método principal: A próxima parte de um programa C é declarar a função main (). A sintaxe para declarar a função principal é:
Sintaxe para declarar o método principal:

```
int main()
{}
```
2. **Declaração da variável**: a próxima parte de qualquer programa C é a declaração da variável. Refere-se às variáveis ​​que devem ser usadas na função. Observe que, no programa C, nenhuma variável pode ser usada sem ser declarada. Também em um programa C, as variáveis ​​devem ser declaradas antes de qualquer operação na função.
**Exemplo**:

```
int main()
{
    
    int a;
    
}
```

2. **Corpo**: o corpo de uma função no programa C, refere-se às operações que são realizadas nas funções. Pode ser qualquer coisa como manipulações, pesquisa, classificação, impressão, etc.
**Exemplo**:

```
int main()
{
    int a;

    printf("%d", a);
}
```
2. **Instrução de retorno**: a última parte de qualquer programa C é a instrução de retorno. A instrução de retorno se refere ao retorno dos valores de uma função. Esta instrução de retorno e valor de retorno dependem do tipo de retorno da função. Por exemplo, se o tipo de retorno for nulo, não haverá instrução de retorno. Em qualquer outro caso, haverá uma instrução de retorno e o valor de retorno será do tipo do tipo de retorno especificado.
**Exemplo**:

```
int main()
{
    int a;

    printf("%d", a);

    return 0;
}
```

2. **Escrevendo o primeiro programa**:
A seguir está o primeiro programa em C

```
#include <stdio.h>
int main(void)
{
    printf("GeeksQuiz");
    return 0;
}
```
Vamos analisar o programa linha por linha.

**Linha 1**: [#include <stdio.h>] Em um programa C, todas as linhas que começam com # são processadas por um pré-processador que é um programa invocado pelo compilador. Em um termo muito básico, o pré-processador pega um programa C e produz outro programa C. O programa produzido não possui linhas começando com #, todas essas linhas são processadas pelo pré-processador. No exemplo acima, o pré-processador copia o código pré-processado de stdio.h para nosso arquivo. Os arquivos .h são chamados de arquivos de cabeçalho em C. Esses arquivos de cabeçalho geralmente contêm declarações de funções. Precisamos de stdio.h para a função printf () usada no programa.

**Linha 2** [int main (void)] Deve haver um ponto de partida de onde a execução do programa C compilado começa. Em C, a execução normalmente começa com a primeira linha de main (). O vazio escrito entre colchetes indica que o principal não tem nenhum parâmetro (veja isto para mais detalhes). main () pode ser escrito para receber parâmetros também. Estaremos cobrindo isso em posts futuros.
O int foi escrito antes de main indicar o tipo de retorno de main (). O valor retornado por main indica o status de encerramento do programa. Veja esta postagem para mais detalhes sobre o tipo de devolução.

**Linha 3 e 6**: [{e}] Na linguagem C, um par de chaves definem o escopo e são usados ​​principalmente em funções e instruções de controle como if, else, loops. Todas as funções devem começar e terminar com chaves.

**Linha 4** [printf (“GeeksQuiz”); ] printf () é uma função de biblioteca padrão para imprimir algo na saída padrão. O ponto-e-vírgula no final de printf indica o término da linha. Em C, um ponto e vírgula é sempre usado para indicar o final de uma instrução.

**Linha 5** [retorno 0; ] A instrução de retorno retorna o valor de main (). O valor retornado pode ser usado por um sistema operacional para saber o status de encerramento do seu programa. O valor 0 normalmente significa encerramento bem-sucedido.

# **Como executar o programa acima:**

Para executar o programa acima, precisamos ter um compilador para compilar e executar nossos programas. Existem certos compiladores online como https://www.onlinegdb.com/online_c_compiler, http://ideone.com/ ou http://codepad.org/ que podem ser usados ​​para iniciar C sem instalar um compilador.
Windows: Existem muitos compiladores disponíveis gratuitamente para a compilação de programas C como Code Blocks e Dev-CPP. Recomendamos fortemente o Code Blocks.
Linux: para o Linux, o gcc vem com o Linux, os Code Blocks também podem ser usados ​​com o Linux.

**Escreva comentários se encontrar algo incorreto ou se quiser compartilhar mais informações sobre o tópico discutido acima**