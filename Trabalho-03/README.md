# TRABALHO 3 - LISTAS ENCADEADAS

## Sistema de Controle de Participação de Alunos Bolsistas em Projetos

Este trabalho consiste na implementação de um sistema de controle de participação de alunos bolsistas em projetos, utilizando listas encadeadas. O sistema deve permitir o cadastro de alunos, professores, projetos e vínculos entre eles, além de gerar relatórios sobre a alocação dos alunos em cada projeto.

### Funcionalidades do programa:

1. **Cadastro de alunos**:
   - É possível incluir alunos e listar todos os alunos cadastrados.
   - Informações armazenadas: número de matrícula, nome e telefone.

2. **Cadastro de projetos**:
   - É possível incluir projetos e listar todos os projetos cadastrados.
   - Informações armazenadas: código do projeto, descrição, tipo (ensino, pesquisa ou extensão), orçamento aprovado, orçamento atual disponível e professor coordenador.

3. **Cadastro de vínculos (alunos em projetos)**:
   - É possível incluir, excluir e listar vínculos entre alunos e projetos.
   - Informações armazenadas: aluno vinculado, projeto e valor mensal da bolsa.

4. **Cadastro de professores**:
   - É possível incluir professores e listar todos os professores cadastrados.
   - Informações armazenadas: código do professor, nome e departamento.

5. **Vinculação de alunos a projetos**:
   - Ao criar um vínculo, o sistema verifica se o orçamento disponível do projeto cobre o pagamento da bolsa por 12 meses.
   - O orçamento disponível do projeto é atualizado automaticamente ao incluir ou excluir vínculos.

6. **Exclusão de vínculos**:
   - Ao excluir um vínculo, o sistema recalcula o orçamento disponível do projeto com base no número de meses restantes da bolsa que não serão pagos.

7. **Relatório de projetos**:
   - Para cada projeto, o sistema imprime:
     - Código do projeto;
     - Tipo do projeto;
     - Nome do professor coordenador;
     - Orçamento atual disponível;
     - Lista de alunos vinculados (se houver).
   - Caso nenhum aluno esteja vinculado, a mensagem "não há alunos vinculados a este projeto" é exibida.

### Restrições:

1. Um aluno só pode ser vinculado a um projeto se houver orçamento disponível para 12 meses de bolsa.
2. O orçamento do projeto é atualizado ao criar ou excluir vínculos.
3. O sistema não armazena duplicidade de informações, usando ponteiros para alunos, projetos e professores cadastrados.
4. Um vínculo só pode ser criado para alunos e projetos previamente cadastrados.
5. Um projeto só pode ser coordenado por um professor previamente cadastrado.

### Estrutura do programa:

- **Listas encadeadas**: Todos os dados (alunos, projetos, professores e vínculos) são armazenados em listas encadeadas, possibilitando a inclusão, remoção e busca dinâmica.
- **Structs alocadas dinamicamente**: Todas as estruturas de dados são alocadas dinamicamente, conforme necessário.
- **Menu de opções**: O programa apresenta um menu para o usuário escolher as ações desejadas (cadastrar, listar, vincular, excluir, etc.).

### Funções esperadas:

1. **Função de alocação de listas**:
   - Implementação de listas encadeadas para alunos, professores, projetos e vínculos.

2. **Funções de cadastro**:
   - Funções para incluir alunos, professores e projetos.

3. **Funções de vinculação**:
   - Funções para vincular alunos a projetos e excluir vínculos.

4. **Funções de atualização de orçamento**:
   - Funções para atualizar o orçamento disponível dos projetos ao criar ou excluir vínculos.

5. **Função de relatório**:
   - Função que gera o relatório de projetos e seus vínculos.

### Observações para este trabalho:

- **Data da entrega**: 04 de novembro, até as 23h.
- **Listas encadeadas**: Os dados devem ser armazenados obrigatoriamente em listas encadeadas (simples ou duplas).
- **Organização do código**: O código deve ser organizado em diferentes arquivos e funções, como por exemplo:
  - `main.c`, `lista.c`, `lista.h`, `menu.c`, `menu.h`.
- **Entrega**: Enviar os arquivos `.c` e `.h` (não anexar executáveis) para o e-mail `deise@inf.ufsm.br`.
- **Trabalho em grupo**: Trabalho em grupos de até 2 alunos. Enviar um e-mail por dupla, identificando a disciplina, o nome dos alunos e o número do trabalho (Trabalho 3).
- **Erros de compilação**: Trabalhos com erros de compilação não serão corrigidos.
- **Funções e passagem de parâmetros**: A solução deve fazer uso de funções e passagem de parâmetros. O `main` deve chamar as funções apropriadas e receber os retornos.
- **Variáveis globais**: Não devem ser usadas variáveis globais.
- **IDE**: O professor usará Dev-C ou Code Blocks para corrigir o trabalho. Certifique-se de que o arquivo compila corretamente em uma dessas IDEs.
- **Questionamentos**: Os alunos podem ser chamados para responder a questionamentos sobre o trabalho entregue, o que fará parte da nota.
- **Arquivo README**: Juntamente com o trabalho, deve ser entregue um arquivo `readme.txt` que descreva sucintamente o que foi e o que não foi implementado.
- **Peso do trabalho**: Verificar no site da disciplina em “Avaliação”.
