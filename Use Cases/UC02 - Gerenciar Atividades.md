# Especificação de Caso de Uso Gametask

## CDU04 - Gerenciar Atividades

| Índice Geral                        |
| :---------------------------------- |
| [Cadastrar Atividade](#cadastro)    |
| [Visualizar Atividade](#visualizar) |
| [Editar Atividade](#editar)         |
| [Concluir Atividade](#concluir)     |

------

<a name='cadastro'></a>

### 1 Cadastrar Atividade

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

O usuário poderá cadastrar uma nova atividade.

<a name='atores1'></a>

#### 1.2 Atores

1. Estudante.

<a name='pre1'></a>

#### 1.3 Precondições

#####  1.3.1 Está Autenticado

O usuário deve está autenticado em sua conta para efetuar a ação.

#####  1.3.2 Disciplina cadastrada

O usuário deve ter disciplina(s) cadastrada(s).

#####  1.3.3 Projeto cadastrado

O usuário deve ter projeto(s) cadastrado(s).

<a name='pos1'></a>

#### 1.4 Pós-condições

##### 1.4.1 Cadastro Efetuado

1. O sistema salva as informações inseridas e cadastra uma nova atividade.

2. O sistema redireciona o usuário de volta à página que solicitou a ação.

<a name='ext1'></a>

#### 1.5 Pontos de Extensão

##### 1.5.1 Concluir Atividade

A definir.

##### 1.5.2 Desistir da Atividade

A definir.

##### 1.5.3 Concluir afazer

A definir.

<a name='fluxos1'></a>

#### 1.6 Fluxos de Evento

##### 1.6.1 Fluxo Básico

1. O usuário clica no link "Nova Atividade" na tela de Visualizar Atividade ou no link "Criar nova" na aba atividades da Dashboard;

2. O sistema gera uma janela flutuante com a opção "Disciplina" na aba "Modelos" pré-selecionada;

3. O sistema mostra 3 campos de inserção, uma caixa de seleção e dois botões na aba "Cadastrar Atividade"

4. O estudante preenche o campo "Nome" com o nome que identifique a atividade;

5. O estudante seleciona uma disciplina pré-cadastrada na caixa de seleção "Disciplina";

6. O estudante preenche o campo "Prazo" com a data de entrega da atividade;

7. O estudante preenche o campo "Descrição" com uma breve descrição da atividade;

8. O sistema gera 2 campos de inserção e dois botões na aba "Lista de Tarefas";

9. O estudante preenche o campo "Tarefa" com o nome da tarefa;

10. O estudante preenche o campo "Descrição da Tarefa" com uma breve descrição da tarefa referida;

11. O estudante pressiona o botão "Confirmar" na aba "Cadastrar Atividade".

    

##### 1.6.2 Fluxos Alternativos

###### 1.6.2.1 Adicionar outra Tarefa

Após o passo 10 do fluxo básico:

1. O usuário pressiona o botão "+" logo abaixo do ultimo campo de inserção da aba "Lista de Tarefas";
2. O sistema gera mais um conjunto de campos e botões composto por mais um campo "Tarefa", um campo "Descrição da Tarefa" e um botão "x" relacionado à essa dupla de campos;
3. Fim do fluxo alternativo;

Retorna ao passo 9 do fluxo básico.

###### 1.6.2.2 Remover uma Tarefa

Após o passo 10 do fluxo básico:

1. O usuário pressiona o botão "x" logo ao lado dos campos de inserção que deseja remover da aba "Lista de Tarefas";
2. O sistema remove da tela os campos de inserção escolhidos e descarta seus conteúdos;
3. Fim do fluxo alternativo;

Retorna a qualquer momento do fluxo básico.

###### 1.6.2.3 Cadastrar Atividade sem Tarefas

Após o passo 8 do fluxo básico:

1. O usuário pressiona o botão "x" logo ao lado dos campos de inserção que deseja remover da aba "Lista de Tarefas";
2. O sistema remove da tela os campos de inserção escolhidos e descarta seus conteúdos;
3. O estudante pressiona o botão "Confirmar" na aba "Cadastrar Atividade".
4. O sistema gera uma nova tela flutuante pedindo a confirmação do cadastramento de uma Atividade sem Tarefas;
5. O usuário pressiona o botão "Confirmar";
6. Fim do fluxo alternativo;

Retorna a qualquer momento do fluxo básico.

###### 1.6.2.4 Modelo Projeto

A qualquer momento do fluxo básico:

1. O estudante pressiona o botão "Projeto" na aba "Modelos";

2. O sistema mostra três campos de inserção, duas caixas de seleção e dois botões na aba "Cadastrar Atividade";
3. O estudante seleciona uma opção na caixa de seleção "Projeto";
4. Fim do fluxo alternativo.

Retorna ao passo 4 do fluxo básico.

###### 1.6.2.5 Modelo Grupo

A qualquer momento do fluxo básico:

1. O estudante pressiona o botão "Projeto" na aba de "Modelos";

2. O sistema mostra cinco campos de inserção, uma caixa de seleção e dois botões na aba "Cadastrar Atividade";

3. O estudante seleciona uma opção na caixa de seleção "Grupo";

4. Fim do fluxo alternativo.

Retorna ao passo 4 do fluxo básico.



##### 1.6.3 Fluxos de Exceção

###### 1.6.3.1 Campo em Branco

Após o passo 5 do fluxo básico:

1. O sistema informa que há um campo de inserção ou caixa de seleção em branco;

2. Fim do fluxo exceção.

Retorna ao passo 5 do fluxo básico.

###### 1.6.3.2 Prazo Inválido

Após o passo 8 do fluxo básico:

1. O sistema informa que o prazo informado é inválido;

2. Fim do fluxo exceção.

Retorna ao passo 4 do fluxo básico.

<a name='proto1'></a>

#### 1.7 Protótipos de Interface do Caso de Uso

##### 1.7.1 Fluxo Básico

![Modelo Disciplina](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Nivel%202.png)

##### 1.7.2 Fluxo A. (Adicionar outra Tarefa)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.3 Fluxo A. (Remover uma Tarefa)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.4 Fluxo A. (Cadastrar Atividade sem Tarefas)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.5 Fluxo A. (Modelo Projeto)

![Modelo Projeto](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.6 Fluxo A. (Modelo Avulso)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.7 Fluxo E. (Campo em Branco)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.7 Fluxo E. (Prazo Inválido)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)



------



<a name='visualizar'></a>

### 2 Visualizar Atividades

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

O usuário poderá pesquisar e visualizar a sua atividade cadastrada escolhida.

<a name='atores2'></a>

#### 2.2 Atores

1. Estudante.

<a name='pre2'></a>

#### 2.3 Precondições

#####  2.3.1 Está Autenticado

O usuário deve está autenticado em sua conta para efetuar a ação.

#####  2.3.2 Atividade cadastrada

O usuário deve ter atividade(s) cadastrada(s).

<a name='pos2'></a>

#### 2.4 Pós-condições

##### 2.4.1 Visualização

O usuário visualizará todas as informações referentes a atividade escolhida.

<a name='ext2'></a>

#### 2.5 Pontos de Extensão

##### 2.5.1 Editar Atividade

Após o passo 6 do fluxo básico:

1. O estudante clica no link "Editar";
2. O sistema executa o "UC02 - Gerenciar Atividades (3. Editar Atividade)";
3. Fim do Ponto de Extensão.

Retorna ao passo 6 do fluxo básico.

##### 2.5.2 Concluir Atividade

Após o passo 6 do fluxo básico:

1. O estudante pressiona o botão "Concluir";
2. O sistema executa o "UC02 - Gerenciar Atividades (4. Concluir Atividade)";
3. Fim do Ponto de Extensão.

Retorna ao passo 6 do fluxo básico.

##### 2.5.3 Cadastrar Atividade

Após o passo 1 do fluxo básico:

1. O estudante clica no link "Nova atividade";
2. O sistema executa o "UC02 - Gerenciar Atividades (1. Cadastrar Atividade)";
3. Fim do Ponto de Extensão.

Retorna ao passo 6 do fluxo básico.



<a name='fluxos2'></a>

#### 2.6 Fluxos de Evento

##### 2.6.1 Fluxo Básico

1. O estudante seleciona no menu lateral a seção "Atividades" ou clica no cartão "Atividades" na tela inicial;

2. O sistema gera uma aba "Filtros" com um campo de inserção e 3 menus suspensos;

3. O usuário preenche o campo "Pesquisar" com o nome da Atividade a qual deseja buscar;

4. O sistema retorna uma lista de atividades na aba "Resultados" que se encaixam na descrição fornecida;

5. O usuário seleciona o cartão de uma atividade;

6. O sistema gera uma aba "Detalhes" com informações referentes à atividade selecionada;

   

##### 2.6.2 Fluxos Alternativos 

###### 2.6.2.1 Filtrar por Atividades

Após o passo 1 do fluxo básico:

1. O estudante clica no menu suspenso "Atividades";
2. O sistema mostra 5 botões radiais (Todas, Pendentes, Concluídas, Data Crescente e Data Decrescente);
3. O estudante seleciona um dos botões;
4. Fim do Fluxo Alternativo.

Retorna ao passo 4 do fluxo básico.

###### 2.6.2.2 Filtrar por Disciplinas

Após o passo 1 do fluxo básico:

1. O estudante clica no menu suspenso "Disciplinas";
2. O sistema mostra X botões radiais (Tantos quanto o número de Disciplinas cadastradas);
3. O estudante seleciona um dos botões;
4. Fim do Fluxo Alternativo.

Retorna ao passo 4 do fluxo básico.

###### 2.6.2.3 Filtrar por Projetos

Após o passo 1 do fluxo básico:

1. O estudante clica no menu suspenso "Projetos";
2. O sistema mostra X botões radiais (Tantos quanto o número de Projetos cadastrados);
3. O estudante seleciona um dos botões;
4. Fim do Fluxo Alternativo.

Retorna ao passo 4 do fluxo básico.



#### 6.3 Fluxos de Exceção

##### 6.3.1 Sem Atividades Cadastradas

Após o passo 1 do fluxo básico:

1. O sistema gera uma tela com um link "Nova Atividade";
2. O estudante clica no link e executa o Ponto de Extensão "Cadastrar Atividade";
3. Fim do Fluxo de Exceção.

##### 6.3.2 Busca Sem Resultados

Após o passo 3 do fluxo básico:

1. O sistema informa ao usuário que não há atividades que correspondam à busca;
2. Fim do Fluxo de Exceção.

Retorna ao passo 3 do fluxo básico.

##### 6.3.3 Filtro Sem Resultados

Após o passo 3 do fluxo alternativo "Filtrar por ...":

1. O sistema informa ao usuário que não há atividades que correspondam à busca;
2. Fim do Fluxo de Exceção.

Retorna ao passo 3 do fluxo alternativo "Filtrar por ...".



<a name='proto2'></a>

#### 2.7 Protótipos de Interface do Caso de Uso

##### 2.7.1 Fluxo Básico

![Visualizar Atividade](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)



##### 1.7.2 Fluxo A. (Filtrar por Atividades)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Nivel%201.png)

##### 1.7.3 Fluxo A. (Filtrar por Disciplinas)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.4 Fluxo A. (Filtrar por Projetos)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.5 Fluxo E. (Sem Atividades Cadastradas)

![Modelo Projeto](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.6 Fluxo E. (Busca Sem Resultados)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 1.7.7 Fluxo E. (Filtro Sem Resultados)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)



------



<a name='editar'></a>

### 3 Editar Atividade

| Índice Editar                 |
| :---------------------------- |
| [Resumo](#resumo3)            |
| [Atores](#atores3)            |
| [Precondições](#pre3)         |
| [Pós-condições](#pos3)        |
| [Pontos de Extensão](#ext3)   |
| [Fluxos de Eventos](#fluxos3) |
| [Protótipos](#proto3)         |

<a name='resumo3'></a>

#### 3.1 Resumo

O usuário poderá alterar as informações de uma atividade anteriormente cadastrada.



<a name='atores3'></a>

#### 3.2 Atores

1. Estudante.



<a name='pre3'></a>

#### 3.3 Precondições

#####  3.3.1 Está Autenticado

O usuário deve está autenticado em sua conta para efetuar a ação.

#####  3.3.2 Atividade cadastrada

O usuário deve ter atividade(s) cadastrada(s).



<a name='pos3'></a>

#### 3.4 Pós-condições

##### 3.4.1 Atualização

O sistema salva as alterações feitas na atividade;

##### 3.4.2 Visualização

O usuário visualizará todas as informações referentes a atividade escolhida.



<a name='ext3'></a>

#### 3.5 Pontos de Extensão

##### 3.5.1 Visualizar Atividade

Após o passo 1 do fluxo básico:

1. O estudante pressiona o botão "Cancelar";
2. O usuário é redirecionado para a página "Visualizar Atividades".



<a name='fluxos3'></a>

#### 3.6 Fluxos de Evento

##### 3.6.1 Fluxo Básico

1. O usuário clica no link "Editar" na aba "Detalhes";
2. O sistema gera uma janela flutuante com a opção referente ao modelo da Atividade pré-selecionada na aba "Modelos";
3. O sistema mostra 3 campos de inserção, uma caixa de seleção e dois botões na aba "Cadastrar Atividade"
4. O estudante preenche o campo "Nome" com o nome que identifique a atividade;
5. O estudante seleciona o campo referente ao modelo pré-cadastrado na caixa de seleção do modelo escolhido;
6. O estudante preenche o campo "Prazo" com a data de entrega da atividade;
7. O estudante preenche o campo "Descrição" com uma breve descrição da atividade;
8. O sistema gera 2 campos de inserção e dois botões na aba "Lista de Tarefas";
9. O estudante preenche o campo "Tarefa" com o nome da tarefa;
10. O estudante preenche o campo "Descrição da Tarefa" com uma breve descrição da tarefa referida;
11. O estudante pressiona o botão "Confirmar" na aba "Cadastrar Atividade".



##### 3.6.2 Fluxos Alternativos 

###### 3.6.2.1 Adicionar outra Tarefa

Após o passo 10 do fluxo básico:

1. O usuário pressiona o botão "+" logo abaixo do ultimo campo de inserção da aba "Lista de Tarefas";
2. O sistema gera mais um conjunto de campos e botões composto por mais um campo "Tarefa", um campo "Descrição da Tarefa" e um botão "x" relacionado à essa dupla de campos;
3. Fim do fluxo alternativo;

Retorna ao passo 9 do fluxo básico.

###### 3.6.2.2 Remover uma Tarefa

Após o passo 10 do fluxo básico:

1. O usuário pressiona o botão "x" logo ao lado dos campos de inserção que deseja remover da aba "Lista de Tarefas";
2. O sistema remove da tela os campos de inserção escolhidos e descarta seus conteúdos;
3. Fim do fluxo alternativo;

Retorna a qualquer momento do fluxo básico.

###### 3.6.2.3 Cadastrar Atividade sem Tarefas

Após o passo 8 do fluxo básico:

1. O usuário pressiona o botão "x" logo ao lado dos campos de inserção que deseja remover da aba "Lista de Tarefas";
2. O sistema remove da tela os campos de inserção escolhidos e descarta seus conteúdos;
3. O estudante pressiona o botão "Confirmar" na aba "Cadastrar Atividade".
4. O sistema gera uma nova tela flutuante pedindo a confirmação do cadastramento de uma Atividade sem Tarefas;
5. O usuário pressiona o botão "Confirmar";
6. Fim do fluxo alternativo;

Retorna a qualquer momento do fluxo básico.



##### 3.6.3 Fluxos de Exceção

###### 3.6.3.1 Campo em Branco

Após o passo 5 do fluxo básico:

1. O sistema informa que há um campo de inserção ou caixa de seleção em branco;

2. Fim do fluxo exceção.

Retorna ao passo 5 do fluxo básico.

###### 3.6.3.2 Prazo Inválido

Após o passo 8 do fluxo básico:

1. O sistema informa que o prazo informado é inválido;

2. Fim do fluxo exceção.

Retorna ao passo 4 do fluxo básico.



<a name='proto3'></a>

#### 3.7 Protótipos de Interface do Caso de Uso

##### 3.7.1 Fluxo Básico

![Modelo Disciplina](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Nivel%202.png)

##### 3.7.2 Fluxo A. (Adicionar outra Tarefa)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 3.7.3 Fluxo A. (Remover uma Tarefa)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 3.7.4 Fluxo A. (Cadastrar Atividade sem Tarefas)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 3.7.5 Fluxo E. (Campo em Branco)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 3.7.6 Fluxo E. (Prazo Inválido)

![Modelo Avulso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)



------



<a name='concluir'></a>

### 4. Concluir Atividade

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

O usuário poderá concluir uma atividade.

<a name='atores4'></a>

#### 4.2 Atores

1. Estudante.

<a name='pre4'></a>

#### 4.3 Precondições

#####  4.3.1 Está Autenticado

O usuário deve está autenticado em sua conta para efetuar a ação.

#####  4.3.2 Atividade cadastrada

O usuário deve ter atividade(s) cadastrada(s).

<a name='pos4'></a>

#### 4.4 Pós-condições

##### 4.4.1 Atividade Concluída

A atividade é removida da lista de atividades pendentes do usuário.

##### 4.4.2 Pontuação Atribuída

É atribuída a nota nesta atividade ao usuário conforme as regras de negócio "1.2.1 - Sistema de pontuação" e "1.2.2 - Cálculo" do [Documento de Projeto](../Documentation/Projeto.md).

<a name='ext4'></a>

#### 4.5 Pontos de Extensão

##### 4.5.1 Não identificado

Até o momento não foram identificados pontos de extensão para a ação.

<a name='fluxos4'></a>

#### 4.6 Fluxos de Evento

##### 4.6.1 Fluxo Básico

1. O estudante seleciona a atividades que deseja concluir;
2. O sistema retorna os detalhes da atividade;
3. O estudante pressiona o botão "Concluir" na aba "Detalhes";
4. O sistema solicita a confirmação por uma janela flutuante;
5. O estudante confirma a ação pressionando o botão "Confirmar".



##### 4.6.2 Fluxos Alternativos 

###### 4.6.2.1 Desistir da Atividade

Após o passo 2 do fluxo básico:

1. O estudante pressiona o botão "Desistir" na aba "Detalhes";
2. Fim do fluxo alternativo.

Retorna ao passo 4 do Fluxo Básico.



##### 4.6.3 Fluxos de Exceção

###### 4.6.3.1  Concluir Com Tarefas Pendentes

Após o passo 2 do fluxo básico:

1. O sistema desativa o botão "Concluir" na aba "Detalhes";
2. O estudante passa o ponteiro do mouse por cima do botão "Concluir";
3. O sistema gera uma dica informando que existem tarefas pendentes;
4. Fim do fluxo de exceção.

Retorna ao passo 2 do Fluxo Básico.

<a name='proto4'></a>

#### 4.7 Protótipos de Interface do Caso de Uso

##### 3.7.1 Fluxo Básico

![Modelo Disciplina](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Nivel%201%20%E2%80%93%201.png)

##### 3.7.2 Fluxo A. (Desistir da Atividade)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

##### 3.7.3 Fluxo E. (Concluir Com Tarefas Pendentes)

![F.A. Adicionar outra Tarefa](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)