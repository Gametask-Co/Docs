# Especificação de Caso de Uso Gametask

## CDU04 - Gerenciar Atividades

| Índice Geral                      |
| :-------------------------------- |
| [Cadastrar Atividade](#cadastro)    |
| [Visualizar Atividade](#visualizar) |
| [Editar Atividade](#editar)         |
| [Desistir da Atividade](#desistir)     |

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

O usuário poderá cadastrar um novo grupo.

<a name='atores1'></a>

#### 1.2 Atores

1. Estudante.

<a name='pre1'></a>

#### 1.3 Precondições

#####  1.3.1 Está Autenticado

O usuário deve está autenticado em sua conta para efetuar a ação.

#####  1.3.2 Acesso à página

O usuário deve ter acesso a algumas das páginas que permitem tal operação.

#####  1.3.3 Disciplina cadastrada

O usuário deve ter disciplina(s) cadastrada(s).

#####  1.3.4 Projeto cadastrado

O usuário deve ter projeto(s) cadastrado(s).

<a name='pos1'></a>

#### 1.4 Pós-condições

##### 1.4.1 Cadastro Efetuado

1. O sistema salva as informações inseridas e cadastra uma nova atividade.

2. O sistema redireciona o usuário de volta à página que solicitou a ação.

<a name='ext1'></a>

#### 1.5 Pontos de Extensão

##### 1.5.1 Operação Cancelada

A qualquer momento no fluxo básico:

1. O estudante pressiona o botão cancelar;

2. O sistema redireciona o usuário de volta à página que solicitou a ação.

<a name='fluxos1'></a>

#### 1.6 Fluxos de Evento

##### 1.6.1 Fluxo Básico

1. O estudante pressiona o botão "Disciplina" na aba "Modelos";

2. O sistema mostra três campos de inserção, duas caixas de seleção e dois botões na aba "Cadastrar Atividade"

3. O estudante seleciona uma opção na caixa de seleção "Disciplina";

4. O estudante preenche o campo "Nome" com o nome que identifique a atividade;

5. O estidante preenche o campo "Prazo" com a data final da atividade;

6. O estudante preenche o campo "Descrição" com uma breve descrição da atividade;

7. O estudante preenche na seção "Lista de Afazeres" o nome do afazer e escreve uma breve descrição;

8. O sistema gera uma prévia do conteúdo e mostra ao estudante;

9. O estudante pressiona o botão "Confirmar" na aba "Visualizar".

##### 1.6.2 Fluxos Alternativos 

###### 1.6.2.1 Modelo Projeto

A qualquer momento do fluxo básico:

1. O estudante pressiona o botão "Projeto" na aba "Modelos";

2. O sistema mostra três campos de inserção, duas caixas de seleção e dois botões na aba "Cadastrar Atividade";

3. O estudante seleciona uma opção na caixa de seleção "Projeto";

4. Fim do fluxo alternativo.

Retorna ao passo 4 do fluxo básico.

###### 1.6.2.2 Modelo Grupo

A qualquer momento do fluxo básico:

1. O estudante pressiona o botão "Projeto" na aba de "Modelos";

2. O sistema mostra cinco campos de inserção, uma caixa de seleção e dois botões na aba "Cadastrar Atividade";

3. O estudante seleciona uma opção na caixa de seleção "Grupo";

4. Fim do fluxo alternativo.

Retorna ao passo 4 do fluxo básico.

###### 1.6.2.3 Adicionar Afazer

Após o passo 7 do fluxo básico:

1. O estudante pressiona o botão "+" na aba "Cadastrar Atividade" na seção "Lista de Afazeres";

2. O sistema cria mais dois campos de inserção e um botão de remoção;

3. Fim do fluxo alternativo.

Retorna ao passo 7 do fluxo básico.

###### 1.6.2.4 Remover Afazer

Após o passo 7 do fluxo básico:

1. O estudante pressiona o botão "x" na aba "Cadastrar Atividade" na seção "Lista de Afazeres";

2. O sistema remove os dois campos de inserção aos quais o botão de remoção era ligado;

3. Fim do fluxo alternativo.

Retorna ao passo 8 do fluxo básico.

##### 1.6.3 Fluxos de Exceção

###### 1.6.3.1 Campo em Branco

Após o passo 5 do fluxo básico:

1. O sistema informa que há um campo de inserção ou caixa de seleção em branco;

2. Fim do fluxo exceção.

Retorna ao passo 5 do fluxo básico.

##### 1.6.3.2 Prazo Inválido

Após o passo 8 do fluxo básico:

1. O sistema informa que o prazo informado é inválido;

2. Fim do fluxo exceção.

Retorna ao passo 4 do fluxo básico.

<a name='proto1'></a>

#### 1.7 Protótipos de Interface do Caso de Uso

##### 1.7.1 Não criado

![]()

##### 1.7.2 Não criado

![]()

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

O usuário poderá ver todas as suas atividades em uma lista.

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

O usuário visualizar todas as informações da atividade escolhida.

<a name='ext2'></a>

#### 2.5 Pontos de Extensão

##### 2.5.1 Não identificado

Até o momento não foram identificados pontos de extensão para a ação.

<a name='fluxos2'></a>

#### 2.6 Fluxos de Evento

##### 2.6.1 Fluxo Básico

1. O estudante seleciona a opção atividades;

2. O sistema mostra um filtro;

3. O usuário preenche o filtro e busca;

4. O sistema retorna uma lista de atividades;

5. O usuário seleciona uma atividade;

6. O sistema mostra os detalhes e informações da atividade;

##### 2.6.2 Fluxos Alternativos 

###### 2.6.2.1  Não identificado

Não foram identificados até o momento fluxos alternativos para a ação.

#### 6.3 Fluxos de Exceção

##### 6.3.1 Não há atividades

Após o passo 3 do fluxo básico:

1. O sistema não retorna nenhuma atividade;

<a name='proto2'></a>

#### 2.7 Protótipos de Interface do Caso de Uso

##### 2.7.1 Título da imagem

![]()

------

<a name='editar'></a>

### 3 Editar Atividade

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

O usuário poderá  alterar todas informações de uma atividade anteriormente cadastrada.

<a name='atores3'></a>

#### 3.2 Atores

1. Estudante.
   
<a name='pre3'></a>

#### 3.3 Precondições

#####  3.3.1 Acesso à página

O usuário deve ter acesso a página "Disciplinas".

##### 3.3.2 Ter atividades

O usuário necessita ter atividades cadastradas.

<a name='pos3'></a>

#### 3.4 Pós-condições

##### 3.4.1 Visualização

1. O sistema salva as alterações feitas na atividade;

2. O usuário é redirecionado para a página "Visualizar Atividades".

<a name='ext3'></a>

#### 3.5 Pontos de Extensão

##### 3.5.1 Cancelar edição

Após o passo 1 do fluxo básico:

1. O estudante pressiona o botão "Cancelar";

2. O usuário é redirecionado para a página "Visualizar Atividades".

<a name='fluxos3'></a>

#### 3.6 Fluxos de Evento

##### 3.6.1 Fluxo Básico

1. O estudante seleciona a opção de visualizar atividades";

2. O sistema mostra um filtro e uma lista de atividades;

3. O estudante seleciona uma atividade;

4. Osistema abre a descrição da atividade;

5. O usuario seleciona a opção de edição;

6. O sistema retorna o formulario preenchido com as informações atuais da atividade;

7. O usuário altera a informação que deseja e seleciona a opção de salvar;

8. O sistema retorna para a página 'Visualizar atividades'.

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

<a name='desistir'></a>

### 4 Desistir da Atividade

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

O usuário poderá remover da sua lista de atividades uma atividade.

<a name='atores4'></a>

#### 4.2 Atores

1. Estudante.

<a name='pre4'></a>

#### 4.3 Precondições

#####  4.3.1 Acesso à página

O usuário deve ter acesso a página de disciplinas.

##### 4.3.2 Ter atividades cadastradas

O usuário dete ter atividades cadastradas.

<a name='pos4'></a>

#### 4.4 Pós-condições

##### 4.4.1 Atividade é removida

A atividade é removida da lista de atividades do usuário.

##### 4.4.2 Nota atribuída

É atribuida a nota nesta atividade ao usuário conforme a regra de negócio 5.2.1 - Sistema de pontuação e 5.2.2 - Cálculo

<a name='ext4'></a>

#### 4.5 Pontos de Extensão

##### 4.5.1 Não identificado

Até o momento não foram identificados pontos de extensão para a ação

<a name='fluxos4'></a>

#### 4.6 Fluxos de Evento

##### 4.6.1 Fluxo Básico

1. O estudante seleciona a opção atividades;

2. O sistema mostra um filtro;

3. O usuário preenche o filtro e busca;

4. O sistema retorna uma lista de atividades;

5. O usuário seleciona uma atividade;

6. O sistema retorna os detalhes da atividade;

7. O usuário seleciona a opção desistir;

8. O sistema solicita a confirmação;

9. O usuário confirma a ação;

10. O sistema retira a atividade da lista do usuário;

##### 4.6.2 Fluxos Alternativos 

###### 4.6.2.1 Não identificado

Não foram identificados até o momento fluxos alternativos para a ação.

##### 4.6.3 Fluxos de Exceção

###### 4.6.3.1  Usuário cancela a desistencia 

Após o passo 8 do fluxo básico:

1. O usuário não confirma a desistencia;

2. O sistema retorna para o detalhamento da atividade;

<a name='proto4'></a>

#### 4.7 Protótipos de Interface do Caso de Uso

##### Não criado

![]()