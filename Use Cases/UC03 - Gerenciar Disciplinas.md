# Especificação de Caso de Uso Gametask

## CDU04 - Gerenciar Disciplinas

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

O usuário poderá cadastrar uma disciplina.

<a name='atores1'></a>

#### 1.2 Atores

1. Estudante.

<a name='pre1'></a>

#### 1.3 Precondições

#####  1.3.1 Está Autenticado

O usuário deve está autenticado em sua conta para efetuar a ação.

#####  1.3.2 Acesso à página

O usuário deve ter acesso a algumas das páginas que permitem tal operação.

<a name='pos1'></a>

#### 1.4 Pós-condições

##### 1.4.1 Cadastro Efetuado

1. O sistema salva as informações inseridas e cadastra a nova discipina;

2. O sistema redireciona o usuário de volta à página que solicitou a ação;

<a name='ext1'></a>

#### 1.5 Pontos de Extensão

##### 1.5.1 Operação Cancelada

1. O estudante pressiona o botão cancelar;

2. O sistema redireciona o usuário de volta à página que solicitou a ação.

<a name='fluxos1'></a>

#### 1.6 Fluxos de Evento

##### 1.6.1 Fluxo Básico

1. O estudante pressiona o botão "Disciplina" na aba "Modelos";

2. O sistema mostra três campos de inserção, duas caixas de seleção e dois botões na aba "Cadastrar Disciplina";

3. O sistema retorna um formulario de cadastro de  disciplina;

4. O estudante preenche o formulario e salva;

5. O sistema confirma a realização da operação e retorna para a página de disciplinas; 

##### 1.6.2 Fluxos Alternativos 

###### 1.6.2.1  Não identificado

Não foram identificados fluxos alternativos até o momento.

##### 1.6.3 Fluxos de Exceção

###### 1.6.3.1 Campo em Branco

Após o passo 5 do fluxo básico:

1. O sistema informa que há um campo de inserção ou caixa de seleção em branco;

2. Fim do fluxo exceção.

Retorna ao passo 5 do fluxo básico.

<a name='proto1'></a>

#### 1.7 Protótipos de Interface do Caso de Uso

##### 1.7.1 Não criado

![]()

##### 1.7.2 Não criado

![]()

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

O usuário poderá ver todas as suas disciplinas cadastradas.

<a name='atores2'></a>

#### 2.2 Atores

1. Estudante.

<a name='pre2'></a>

#### 2.3 Precondições

#####  2.3.1 Acesso à página

O usuário deve ter acesso a página de disciplinas.

##### 2.3.2  Ter disciplinas cadastradas

O usuário deve ter disciplinas cadastradas.

<a name='pos2'></a>

#### 2.4 Pós-condições

##### 2.4.1 Visualização

O usuário visualizar todas as informações da disciplina escolhida.

<a name='ext2'></a>

#### 2.5 Pontos de Extensão

##### 2.5.1 Não identificado

Até o momento não foram identificados pontos de extensão para a ação.

<a name='fluxos2'></a>

#### 2.6 Fluxos de Evento

##### 2.6.1 Fluxo Básico

1. O estudante seleciona a opção Disciplinas;

2. O sistema mostra um filtro e uma lista de disciplinas;

3. O estudante seleciona uma disciplina;

4. O sistema mostra os detalhes da disciplina;

##### 2.6.2 Fluxos Alternativos 

###### 2.6.2.1  Não identificado

Não foram identificados até o momento fluxos alternativos para a ação.

#### 6.3 Fluxos de Exceção

##### 6.3.1 Não identificado

Não foram identificados fluxos de exceção até o momento

<a name='proto2'></a>

#### 2.7 Protótipos de Interface do Caso de Uso

##### 2.7.1 Título da imagem

![]()

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

O usuário deseja editar informações de um projeto.

<a name='atores3'></a>

#### 3.2 Atores

1. Estudante.
   
<a name='pre3'></a>

#### 3.3 Precondições

#####  3.3.1 Acesso à página

O usuário deve ter acesso a página "Disciplinas".

##### 3.3.2 Ter Disciplinas

O usuário necessita ter disciplinas cadastradas.

<a name='pos3'></a>

#### 3.4 Pós-condições

##### 3.4.1 Visualização

1. O sistema salva as alterações feitas na disciplinas;

2. O usuário é redirecionado para a página "Visualizar Disciplinas".

<a name='ext3'></a>

#### 3.5 Pontos de Extensão

##### 3.5.1 Cancelar edição

Após o passo 1 do fluxo básico:

1. O estudante pressiona o botão "Cancelar";

2. O usuário é redirecionado para a página "Visualizar Disciplinas".

<a name='fluxos3'></a>

#### 3.6 Fluxos de Evento

##### 3.6.1 Fluxo Básico

1. O estudante seleciona a opção de visualizar Disciplinas";

2. O sistema mostra um filtro e uma lista de Disciplinas;

3. O estudante seleciona uma Disciplina;

4. O sistema abre as informações da disciplina;

5. O usuario seleciona a opção de edição;

6. O sistema retorna o formulario preenchido com as informações atuais da disciplina;

7. O usuário altera a informação que deseja e seleciona a opção de salvar;

8. O sistema retorna para a página 'Visualizar disciplinas'. 

##### 3.6.2 Fluxos Alternativos 

###### 3.6.2.1 Não identificado

Até o momento não foram encontrados fluxos alternativos.

##### 3.6.3 Fluxos de Exceção

###### 3.6.3.1 Campo em Branco

Após o passo 6 do fluxo básico:

1. O sistema informa que há um campo de inserção ou caixa de seleção em branco;

2. Fim do fluxo exceção.

Retorna ao passo 6 do fluxo básico.

<a name='proto3'></a>

#### 3.7 Protótipos de Interface do Caso de Uso

##### 3.7.1 Projeto

![]()

------

<a name='trancar'></a>

### 4 Trancar disciplina

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

O usuário poderá remover da sua lista de disciplinas uma disciplina.

<a name='atores4'></a>

#### 4.2 Atores

1. Estudante.

<a name='pre4'></a>

#### 4.3 Precondições

#####  4.3.1 Acesso à página

O usuário deve ter acesso a página de disciplinas.

##### 4.3.2  Ter disciplinas cadastradas

O usuário dete ter disciplinas cadastradas.

<a name='pos4'></a>

#### 4.4 Pós-condições

##### 4.4.1 Disciplina é removida

A disciplina é removida da lista de disciplinas do usuário.

<a name='ext4'></a>

#### 4.5 Pontos de Extensão

##### 4.5.1 Não identificado

Até o momento não foram identificados pontos de extensão para a ação

<a name='fluxos4'></a>

#### 4.6 Fluxos de Evento

##### 4.6.1 Fluxo Básico

1. O estudante seleciona a opção Disciplina;

2. O sistema mostra um filtro e uma lista de disciplinas;

3. O usuário seleciona uma disciplina;

4. O sistema retorna a descrição da disciplina;

5. O usuário seleciona a opção trancar disciplina;

6. O sistema solicita a confirmação;

7. O usuário confirma a ação;

8. O sistema retira a disciplina da lista do usuário; 

##### 4.6.2 Fluxos Alternativos 

###### 4.6.2.1 Busca pelo filtro

Após o passo 2 do fluxo básico:

1. O usuário preenche o filtro e busca;

2. O sistema retorna as disciplinas referentes a busca;

3. Retorna ao fluxo básico no passo 3.

##### 4.6.3 Fluxos de Exceção

###### 4.6.3.1  Usuário cancela o trancamento 

Após o passo 8 do fluxo básico:

1. O usuário não confirma o trancamento;

2. O sistema retorna para o detalhamento da atividade;

<a name='proto4'></a>

#### 4.7 Protótipos de Interface do Caso de Uso

##### Não criado

![]()