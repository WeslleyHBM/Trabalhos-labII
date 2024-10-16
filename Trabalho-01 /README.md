# TRABALHO 1 - LABORATÓRIO DE PROGRAMAÇÃO 2

## Questões

### 1. SELEÇÃO

Escreva um programa em C para calcular se um aluno foi aprovado ou reprovado com base nas notas de duas provas (P1 e P2). O critério de aprovação é:
- Se a média de P1 e P2 for maior ou igual a 5.0 **e** nenhuma das duas notas for inferior a 3.0, o aluno está aprovado diretamente.
- Caso contrário, o aluno faz uma terceira prova (P3), e a média final é calculada considerando a maior nota entre P1 e P2 junto com a nota de P3. O aluno será aprovado se essa média for maior ou igual a 5.0.

**Entrada:** 
- Notas das provas (P1, P2 e, se necessário, P3).
  
**Saída:** 
- Média final do aluno e status ("Aprovado" ou "Reprovado").

### 2. REPETIÇÃO

Escreva um programa em C que leia **vários conjuntos** de três valores reais. Para cada conjunto, o programa deve calcular e mostrar:
- Soma dos três valores;
- Produto dos três valores;
- Média dos três valores.

O programa deve encerrar a execução quando os valores do conjunto não estiverem em ordem crescente.

### 3. VETORES

Escreva um programa em C que:
- Leia um vetor de inteiros de tamanho 5;
- Inverta e imprima o vetor;
- Ordene e imprima o vetor em ordem decrescente;
- Calcule e imprima:
  1. O maior valor do vetor;
  2. O menor valor do vetor;
  3. A média dos valores do vetor;
  4. A quantidade de valores que são maiores que a média calculada.

Cada um dos itens acima deve ser implementado em uma função separada.

### 4. MATRIZES

Escreva um programa em C para armazenar dados COVID de vários municípios em uma matriz de inteiros de tamanho `m x 6`. Os dados são organizados da seguinte forma:
- Primeira coluna: código do município;
- Segunda coluna: quantidade de habitantes do município;
- Terceira coluna: total de casos confirmados;
- Quarta coluna: total de óbitos;
- Quinta coluna: incidência de casos a cada 100 mil habitantes;
- Sexta coluna: mortalidade a cada 100 mil habitantes.

O programa deve:
- Ler e preencher as quatro primeiras colunas da matriz;
- Calcular e armazenar a incidência de casos e a mortalidade nas duas últimas colunas;
- Imprimir toda a matriz;
- Mostrar o código do município com maior mortalidade;
- Mostrar o código do município com maior incidência de casos.

Cada um dos itens deve ser implementado em uma função separada.

### 5. STRUCTS

Escreva um programa em C para armazenar e processar dados de uma pesquisa de campo sobre leitura de livros no ano de 2023. Os dados de cada entrevistado (idade e quantidade de livros lidos) devem ser armazenados em um vetor de `struct`.

```c
struct usuario {
    int idade;
    int qtdade;
};
typedef struct usuario Usuario;
```

## Observações

- **Data da entrega:** 23 de setembro, até as 23h59m.
- **Formato da entrega:** enviar os arquivos fonte `.c` (não anexar arquivos executáveis) para o e-mail `deise@inf.ufsm.br`. 
  - Um arquivo `.c` para cada questão do trabalho.
- **Trabalho em grupos de 2 alunos.** Enviar um e-mail por dupla.
- **Confirmação do envio:** caso não receba confirmação do recebimento do e-mail em 24 horas, contate o professor novamente. Reclamações posteriores sobre possíveis problemas no envio do e-mail **não serão aceitas**.
- **Plágio:** cópias da internet e/ou de colegas de outras duplas **anulam a nota** de todos os envolvidos.
- **Compilação:** trabalhos com erros de compilação **não serão corrigidos**.
- O professor usará o **Dev-C++** ou **Code::Blocks** para corrigir os trabalhos. Certifique-se de que seu código compila corretamente em uma dessas IDEs.
- **Estrutura do código:** evite escrever toda a solução dentro do `main`. Utilize funções separadas sempre que possível.
- **Não utilizar variáveis globais.**
- Todas as questões devem ser compiláveis e executáveis, permitindo entrada de dados para a correção.
- **Peso do trabalho:** verificar no site da disciplina.
