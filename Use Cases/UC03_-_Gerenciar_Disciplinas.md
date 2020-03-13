# Especificação de Caso de Uso Gametask

## CDU03 - Gerenciar Disciplinas

| Índice Geral                      |
| :-------------------------------- |
| [Cadastrar Disciplina](#cadastro)    |
| [Visualizar Disciplina](#visualizar) |
| [Editar Disciplina](#editar)         |
| [Trancar Disciplina](#trancar)     |

------

<a name='cadastro'></a>

### 1 Cadastrar Disciplina

| Índice Cadastrar              |
| :---------------------------- |
| [Resumo](#resumo1)            |
| [Atores](#atores1)            |
| [Precondições](#pre1)         |
| [Pós-condições](#pos1)        |
| [Pontos de Extensão](#ext1)   |
| [Fluxos de Eventos](#fluxos1) |
| [Protótipos](#proto1)         |

<a name='resumo1'></a>

#### 1.1 Resumo

O usuário poderá cadastrar uma nova disciplina.

<a name='atores1'></a>

#### 1.2 Atores

1. Estudante.

<a name='pre1'></a>

#### 1.3 Precondições

#####  1.3.1 Está Autenticado

O usuário deve está autenticado em sua conta para efetuar a ação.

<a name='pos1'></a>

#### 1.4 Pós-condições

##### 1.4.1 Cadastro Efetuado

1. O sistema salva as informações inseridas e cadastra a nova disciplina;

2. O sistema redireciona o usuário de volta à página que solicitou a ação;

<a name='ext1'></a>

#### 1.5 Pontos de Extensão

##### 1.5.1  Adicionar Horários

Durante o passo 12 do fluxo básico:

1. O estudante pressiona o botão "Adicionar Horário" na aba "Horários";
2. O sistema gera uma janela flutuante com uma tabela de horários;
3. O estudante seleciona as células da tabela que satisfaça as condições da sua disciplina;
4. O sistema gera uma janela de confirmação;
5. O estudante pressiona o botão "Confirmar";
6. O sistema grava as informações na tabela de horários da aba "Horários";
7. Fim do ponto de extensão.

Retorna ao passo 13 do fluxo básico.

<a name='fluxos1'></a>

#### 1.6 Fluxos de Evento

##### 1.6.1 Fluxo Básico

1. O usuário clica no link "Nova Disciplina" na tela de Visualizar Disciplina;

2. O sistema gera uma janela flutuante com a opção "Créditos/Horas" na aba "Modelos" pré-selecionada;

3. O sistema mostra 6 campos de inserção, uma caixa de seleção e dois botões na aba "Cadastrar Disciplina";

4. O estudante preenche o campo "Nome" com o nome que identifique a disciplina;

5. O estudante preenche o campo "Código" com um código ou abreviação que identifique a disciplina;

6. O estudante preenche o campo "Sala" com o nome da sala, auditório ou laboratório onde a disciplina ocorre;

7. O estudante preenche o campo "Docente" com o nome do professor(a) que leciona a disciplina;

8. O estudante seleciona a opção "Créditos" na caixa de seleção "Tipo";

9. O estudante preenche o campo "Carga Horária" com a quantidade de créditos que desejar;

10. O estudante preenche o campo "Descrição" com uma breve descrição da disciplina;

11. O sistema gera uma tabela de horários vazia na aba "Horários", um botão "Adicionar Horário" e um aviso de quantos horários à cadastrar ainda existem;

12. O estudante executa o ponto de extensão "Adicionar Horários";

13. O sistema gera um botão "Editar Horário" no lugar do botão "Adicionar Horário" na aba "Horários";

14. O estudante pressiona o botão "Confirmar" na aba "Cadastrar Atividade".

    

##### 1.6.2 Fluxos Alternativos 

###### 1.6.2.1  Tipo Hora

Após o passo 7 do fluxo básico:

1. O estudante seleciona a opção "Horas" na caixa de seleção "Tipo";
2. Fim do fluxo alternativo.

Retorna ao passo 9 do fluxo básico.

###### 1.6.2.2 Modelo Avulso

A qualquer momento do fluxo básico:

1. O estudante pressiona o botão "Avulso" na aba "Modelos";
2. O sistema mostra 4 campos de inserção e dois botões na aba "Cadastrar Disciplina";
3. O estudante preenche o campo "Nome" com o nome que identifique a disciplina;
4. O estudante preenche o campo "Sala" com o nome da sala, auditório ou laboratório onde a disciplina ocorre;
5. Fim do fluxo alternativo.

Retorna ao passo 9 do fluxo básico.



##### 1.6.3 Fluxos de Exceção

###### 1.6.3.1 Campo em Branco

Após o passo 3 do fluxo básico:

1. O sistema informa que há um campo de inserção ou caixa de seleção em branco;

2. Fim do fluxo exceção.

Retorna ao passo 3 do fluxo básico.

###### 1.6.3.2 Carga Horária Inválida

Após o passo 9 do fluxo básico:

1. O sistema informa que a carga horária informada é inválida;

2. Fim do fluxo exceção.

Retorna ao passo 9 do fluxo básico.

###### 1.6.3.3 Conflito de Horários

Após o passo 3 do ponto de extensão "Adicionar Horários":

1. O sistema informa que a célula escolhida já está ocupada;

2. Fim do fluxo exceção.

Retorna ao passo 3 do fluxo básico.



<a name='proto1'></a>

#### 1.7 Protótipos de Interface do Caso de Uso

##### 1.7.1 Fluxo Básico

![Fluxo Básico - Cadastrar Disciplina](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.2 Fluxo A. (Tipo Hora)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.3 Fluxo A. (Modelo Avulso)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.4 Fluxo E. (Campo em Branco)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.5 Fluxo E. (Carga Horária Inválida)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.6 Fluxo E. (Conflito de Horários)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.7 Ponto de Extensão (Adicionar Horários)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)



------

<a name='visualizar'></a>

### 2 Visualizar Disciplinas

| Índice Visualizar             |
| ----------------------------- |
| [Resumo](#resumo2)            |
| [Atores](#atores2)            |
| [Precondições](#pre2)         |
| [Pós-condições](#pos2)        |
| [Pontos de Extensão](#ext2)   |
| [Fluxos de Eventos](#fluxos2) |
| [Protótipos](#proto2)         |

<a name='resumo2'></a>

#### 2.1 Resumo

O usuário poderá pesquisar e visualizar a sua disciplina cadastrada escolhida.

<a name='atores2'></a>

#### 2.2 Atores

1. Estudante.

<a name='pre2'></a>

#### 2.3 Precondições

#####  2.3.1 Está Autenticado

O usuário deve está autenticado em sua conta para efetuar a ação.

#####  2.3.2 Atividade cadastrada

O usuário deve ter disciplina(s) cadastrada(s).

<a name='pos2'></a>

#### 2.4 Pós-condições

##### 2.4.1 Visualização

O usuário visualizará todas as informações referentes a disciplina escolhida.

<a name='ext2'></a>

#### 2.5 Pontos de Extensão

##### 2.5.1 Editar Disciplina

Após o passo 6 do fluxo básico:

1. O estudante clica no link "Editar";
2. O sistema executa o "UC03 - Gerenciar Disciplina (3. Editar Disciplina)";
3. Fim do Ponto de Extensão.

Retorna ao passo 6 do fluxo básico.

##### 2.5.2 Concluir Disciplina

Após o passo 6 do fluxo básico:

1. O estudante pressiona o botão "Concluir";
2. O sistema executa o "UC03 - Gerenciar Disciplina (4. Trancar Disciplina)";
3. Fim do Ponto de Extensão.

Retorna ao passo 6 do fluxo básico.

##### 2.5.3 Cadastrar Disciplina

Após o passo 1 do fluxo básico:

1. O estudante clica no link "Nova Disciplina";
2. O sistema executa o "UC03 - Gerenciar Disciplina (1. Cadastrar Disciplina)";
3. Fim do Ponto de Extensão.

Retorna ao passo 6 do fluxo básico.



<a name='fluxos2'></a>

#### 2.6 Fluxos de Evento

##### 2.6.1 Fluxo Básico

1. O estudante seleciona no menu lateral a seção "Disciplinas";

2. O sistema gera uma aba "Filtros" com um campo de inserção e 1 menus suspensos;

3. O usuário preenche o campo "Pesquisar" com o nome da Disciplina a qual deseja buscar;

4. O sistema retorna uma lista de disciplinas na aba "Resultados" que se encaixam na descrição fornecida;

5. O usuário seleciona o cartão de uma disciplina;

6. O sistema gera uma aba "Detalhes" com informações referentes à disciplina selecionada.

   

##### 2.6.2 Fluxos Alternativos 

###### 2.6.2.1 Filtrar por Disciplinas

Após o passo 1 do fluxo básico:

1. O estudante clica no menu suspenso "Disciplinas";
2. O sistema mostra X botões radiais (Tantos quanto o número de Disciplinas cadastradas);
3. O estudante seleciona um dos botões;
4. Fim do Fluxo Alternativo.

Retorna ao passo 6 do fluxo básico.



#### 2.6.3 Fluxos de Exceção

##### 2.6.3.1 Sem Disciplinas Cadastradas

Após o passo 1 do fluxo básico:

1. O sistema gera uma tela com um link "Nova Disciplina";
2. O estudante clica no link e executa o Ponto de Extensão "Cadastrar Disciplina";
3. Fim do Fluxo de Exceção.

##### 2.6.3.2 Busca Sem Resultados

Após o passo 3 do fluxo básico:

1. O sistema informa ao usuário que não há disciplina que correspondam à busca;
2. Fim do Fluxo de Exceção.

Retorna ao passo 3 do fluxo básico.



<a name='proto2'></a>

#### 2.7 Protótipos de Interface do Caso de Uso

##### 2.7.1 Fluxo Básico

![Visualizar Atividade](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)



##### 2.7.2 Fluxo A. (Filtrar por Disciplinas)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)



##### 2.7.5 Fluxo E. (Sem Disciplinas Cadastradas)

![Modelo Projeto](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 2.7.6 Fluxo E. (Busca Sem Resultados)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)



------

<a name='editar'></a>

### 3 Editar Disciplina

| Índice Editar         |
| :---------------------------- |
| [Resumo](#resumo3)            |
| [Atores](#atores3)           |
| [Precondições](#pre3)         |
| [Pós-condições](#pos3)        |
| [Pontos de Extensão](#ext3)   |
| [Fluxos de Eventos](#fluxos3) |
| [Protótipos](#proto3)         |

<a name='resumo3'></a>

#### 3.1 Resumo

O usuário poderá alterar as informações de uma disciplina anteriormente cadastrada.



<a name='atores3'></a>

#### 3.2 Atores

1. Estudante.
   
   

<a name='pre3'></a>

#### 3.3 Precondições

#####  3.3.1 Está Autenticado

O usuário deve está autenticado em sua conta para efetuar a ação.

#####  3.3.2 Disciplina cadastrada

O usuário deve ter disciplina (s) cadastrada(s).



<a name='pos3'></a>

#### 3.4 Pós-condições

##### 3.4.1 Atualização

O sistema salva as alterações feitas na disciplina;

##### 3.4.2 Visualização

O usuário visualizará todas as informações referentes a disciplina editada.



<a name='ext3'></a>

#### 3.5 Pontos de Extensão

##### 3.5.1 Visualizar Disciplina

Após o passo 11 do fluxo básico:

1. O usuário é redirecionado para a página "Visualizar Disciplina";
2. Fim do ponto de extensão.

##### 3.5.2  Adicionar Horários

Durante o passo 12 do fluxo básico:

1. O estudante pressiona o botão "Adicionar Horário" na aba "Horários";
2. O sistema gera uma janela flutuante com uma tabela de horários;
3. O estudante seleciona as células da tabela que satisfaça as condições da sua disciplina;
4. O sistema gera uma janela de confirmação;
5. O estudante pressiona o botão "Confirmar";
6. O sistema grava as informações na tabela de horários da aba "Horários";
7. Fim do ponto de extensão.

Retorna ao passo 13 do fluxo básico.



<a name='fluxos3'></a>

#### 3.6 Fluxos de Evento

##### 3.6.1 Fluxo Básico

1. O usuário clica no link "Editar" na aba "Detalhes";

2. O sistema gera uma janela flutuante com a opção referente ao modelo da Disciplina pré-selecionada na aba "Modelos";

3. O sistema mostra 6 campos de inserção, uma caixa de seleção e dois botões na aba "Cadastrar Disciplina";

4. O estudante preenche o campo "Nome" com o nome que identifique a disciplina;

5. O estudante preenche o campo "Código" com um código ou abreviação que identifique a disciplina;

6. O estudante preenche o campo "Sala" com o nome da sala, auditório ou laboratório onde a disciplina ocorre;

7. O estudante preenche o campo "Docente" com o nome do professor(a) que leciona a disciplina;

8. O estudante seleciona a opção "Créditos" na caixa de seleção "Tipo";

9. O estudante preenche o campo "Carga Horária" com a quantidade de créditos que desejar;

10. O estudante preenche o campo "Descrição" com uma breve descrição da disciplina;

11. O sistema gera uma tabela de horários e um botão "Editar Horário" na aba "Horários";

12. O estudante executa o ponto de extensão "Adicionar Horários";

13. O estudante pressiona o botão "Confirmar" na aba "Cadastrar Atividade".

    

##### 3.6.2 Fluxos Alternativos 

###### 3.6.2.1  Tipo Hora

Após o passo 7 do fluxo básico:

1. O estudante seleciona a opção "Horas" na caixa de seleção "Tipo";
2. Fim do fluxo alternativo.

Retorna ao passo 9 do fluxo básico.

###### 3.6.2.2 Modelo Avulso

A qualquer momento do fluxo básico:

1. O estudante pressiona o botão "Avulso" na aba "Modelos";
2. O sistema mostra 4 campos de inserção e dois botões na aba "Cadastrar Disciplina";
3. O estudante preenche o campo "Nome" com o nome que identifique a disciplina;
4. O estudante preenche o campo "Sala" com o nome da sala, auditório ou laboratório onde a disciplina ocorre;
5. Fim do fluxo alternativo.

Retorna ao passo 9 do fluxo básico.



##### 3.6.3 Fluxos de Exceção

###### 3.6.3.1 Campo em Branco

Após o passo 3 do fluxo básico:

1. O sistema informa que há um campo de inserção ou caixa de seleção em branco;

2. Fim do fluxo exceção.

Retorna ao passo 3 do fluxo básico.

###### 3.6.3.2 Carga Horária Inválida

Após o passo 9 do fluxo básico:

1. O sistema informa que a carga horária informada é inválida;

2. Fim do fluxo exceção.

Retorna ao passo 9 do fluxo básico.

###### 3.6.3.3 Conflito de Horários

Após o passo 3 do ponto de extensão "Adicionar Horários":

1. O sistema informa que a célula escolhida já está ocupada;

2. Fim do fluxo exceção.

Retorna ao passo 3 do fluxo básico.



<a name='proto3'></a>

#### 3.7 Protótipos de Interface do Caso de Uso

##### 3.7.1 Fluxo Básico

![Fluxo Básico - Cadastrar Disciplina](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 3.7.2 Fluxo A. (Tipo Hora)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 3.7.3 Fluxo A. (Modelo Avulso)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 3.7.4 Fluxo E. (Campo em Branco)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 3.7.5 Fluxo E. (Carga Horária Inválida)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 3.7.6 Fluxo E. (Conflito de Horários)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 3.7.7 Ponto de Extensão (Adicionar Horários)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

------

<a name='trancar'></a>

### 4 Trancar Disciplina

| Índice Concluir               |
| ----------------------------- |
| [Resumo](#resumo4)            |
| [Atores](#atores4)            |
| [Precondições](#pre4)         |
| [Pós-condições](#pos4)        |
| [Pontos de Extensão](#ext4)   |
| [Fluxos de Eventos](#fluxos4) |
| [Protótipos](#proto4)         |

<a name='resumo4'></a>

#### 4.1 Resumo

O usuário poderá remover da sua lista de disciplinas avaliáveis a disciplina escolhida.



<a name='atores4'></a>

#### 4.2 Atores

1. Estudante.

   

<a name='pre4'></a>

#### 4.3 Precondições

#####  4.3.1 Está Autenticado

O usuário deve está autenticado em sua conta para efetuar a ação.

#####  4.3.2 Disciplina cadastrada

O usuário deve ter disciplina(s) cadastrada(s).



<a name='pos4'></a>

#### 4.4 Pós-condições

##### 4.4.1 Disciplina é removida

A disciplina é removida da lista de disciplinas avaliáveis do usuário, mas permanece acessível pelo menu de configurações.



<a name='ext4'></a>

#### 4.5 Pontos de Extensão

##### 4.5.1 Não identificado

Até o momento não foram identificados pontos de extensão para a ação.



<a name='fluxos4'></a>

#### 4.6 Fluxos de Evento

##### 4.6.1 Fluxo Básico

1. O estudante seleciona a disciplina que deseja concluir;

2. O sistema retorna os detalhes da disciplina;

3. O estudante pressiona o botão "Concluir" na aba "Detalhes";

4. O sistema solicita a confirmação por uma janela flutuante;

5. O estudante confirma a ação inserindo o nome da disciplina e pressionando o botão "Confirmar".

   

##### 4.6.2 Fluxos Alternativos 

###### 4.6.2.1 Não identificado

Até o momento não foram identificados fluxos alternativos para a ação.



##### 4.6.3 Fluxos de Exceção

###### 4.6.3.1  Confirmação Incorreta 

Após o passo 5 do fluxo básico:

1. O usuário não informa o nome correto da disciplina;
2. O sistema gera uma dica informando que o nome está incorreto;
3. Fim do fluxo de exceção.

Retorna ao passo 4 do Fluxo Básico.



<a name='proto4'></a>

#### 4.7 Protótipos de Interface do Caso de Uso

##### 4.7.1 Fluxo Básico

![Modelo Disciplina](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 4.7.2 Fluxo E. (Confirmação Incorreta)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

