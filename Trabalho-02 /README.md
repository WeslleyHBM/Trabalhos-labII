# TRABALHO 2 - CAÇA-PALAVRAS

## Alocação Dinâmica de Matrizes

Este trabalho consiste na implementação de um jogo de **Caça-Palavras** em C, utilizando alocação dinâmica de memória para manipular matrizes de caracteres. O programa deve preencher a matriz com um texto fornecido pelo usuário e permitir a busca de palavras, que podem estar dispostas de várias formas na matriz.

### Funcionalidades do programa:

1. **Leitura da dimensão da matriz**:
   - O programa solicita ao usuário a quantidade de linhas `m` e colunas `n` da matriz.

2. **Preenchimento da matriz**:
   - O usuário digita um texto que será armazenado na matriz, caractere por caractere.
   - O preenchimento da matriz é sequencial, ou seja, começa da primeira linha até a última, ignorando espaços em branco do texto.

   **Exemplo:**
   - Tamanho da matriz: 5 x 9
   - Texto digitado: `"Temos um texto usado apenas como exemplo da entrada"`
   - Matriz gerada (sem espaços):
     ```
     1 2 3 4 5 6 7 8 9
     1 T e m o s u m t e
     2 x t o u s a d o a
     3 p e n a s c o m o
     4 e x e m p l o d a
     5 e n t r a d a
     ```

3. **Impressão da matriz**:
   - O programa exibe a matriz gerada de forma organizada.

4. **Busca de palavras**:
   - O usuário pode buscar palavras na matriz.
   - O programa indica se a palavra ocorre nas seguintes direções:
     - **Horizontal direta** (da esquerda para a direita);
     - **Horizontal reversa** (da direita para a esquerda);
     - **Vertical direta** (de cima para baixo);
     - **Vertical reversa** (de baixo para cima);
     - **Diagonal principal direta** (da esquerda superior para a direita inferior);
     - **Diagonal principal reversa** (da direita inferior para a esquerda superior);
     - **Diagonal secundária direta** (da direita superior para a esquerda inferior);
     - **Diagonal secundária reversa** (da esquerda inferior para a direita superior).
   - Além disso, o programa mostra as posições de início e fim da palavra encontrada.

   **Exemplo de saída**:
   - Palavra: `usado`
   - Resultado: A palavra ocorre na **horizontal direta**, iniciando na posição `[2,4]` e terminando na posição `[2,8]`.
   
   - Palavra: `nxet`
   - Resultado: A palavra ocorre na **vertical reversa**, iniciando na posição `[5,2]` e terminando na posição `[2,2]`.
   
   - Palavra: `oapd`
   - Resultado: A palavra ocorre na **diagonal principal direta**, iniciando na posição `[2,3]` e terminando na posição `[5,6]`.

### Funções esperadas no programa:

1. **Alocação da matriz**:
   - Função responsável por alocar dinamicamente a matriz de caracteres com base nas dimensões fornecidas pelo usuário.

2. **Preenchimento da matriz**:
   - Função que armazena os caracteres do texto fornecido na matriz, seguindo a ordem de inserção sem considerar os espaços em branco.

3. **Impressão da matriz**:
   - Função para exibir a matriz de forma estruturada e legível.

4. **Busca de palavras**:
   - Funções separadas para buscar palavras nas diferentes direções (horizontal, vertical, diagonal).

5. **Liberação da matriz**:
   - Função para liberar a memória alocada dinamicamente para a matriz.

### Observações para este trabalho:

- **Data da entrega:** 9 de outubro.
- **Formato da entrega:** Enviar o arquivo fonte `.c` (não anexar executáveis) para o e-mail `deise@inf.ufsm.br`.
- **Trabalho em grupos de até 2 alunos**. Enviar um e-mail por dupla, identificando a disciplina, nome dos alunos e número do trabalho.
- **Erros de compilação:** Trabalhos com erros de compilação não serão corrigidos.
- **Funções e passagem de parâmetros:** É obrigatório fazer uso de funções e passar parâmetros. O `main` deve chamar essas funções e receber os retornos adequados.
- **Uso de variáveis globais não é permitido.**
- **Alocação dinâmica:** A matriz de caracteres deve ser alocada dinamicamente.
- **Funções úteis**: Podem ser usadas as funções `strstr` (para busca de substring) e `strrev` (para reverter strings).
- **Entrega adicional:** Enviar também um arquivo `readme.txt` descrevendo brevemente o que foi implementado e o que não foi implementado.
- **Peso do trabalho:** Verificar no site da disciplina.
