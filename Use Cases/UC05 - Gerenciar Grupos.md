# Especificação de Caso de Uso Gametask

## CDU05 - Gerenciar Grupo

| Índice Geral                    |
| :------------------------------ |
| [Cadastrar Grupo](#cadastro)    |
| [Visualizar Grupo](#visualizar) |
| [Editar Grupo](#editar)         |
| [Concluir Grupo](#concluir)     |

------

<a name='cadastro'></a>

### 1 Cadastrar Grupo

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

O usuário cadastra um novo grupo em sua conta.



<a name='atores1'></a>

#### 1.2 Atores

1. Estudante.

   

<a name='pre1'></a>

#### 1.3 Precondições

#####  1.3.1 Está Autenticado

O usuário deve está autenticado em sua conta para efetuar o cadastramento.

#####  1.3.2 Acesso à página

O usuário deve ter acesso aos links que trazem a página de cadastramento.

##### 1.3.3 Projeto cadastrado

O usuário deve ter projeto(s) cadastrado(s).



<a name='pos1'></a>
#### 1.4 Pós-condições

##### 1.4.1 Cadastro Efetuado

1. O sistema salva as informações inseridas e cadastra um novo grupo;

2. O sistema redireciona o usuário de volta à pagina que solicitou a ação.

   

<a name='ext1'></a>
#### 1.5 Pontos de Extensão

##### 1.5.1 Operação Cancelada

1. O estudante pressiona o botão cancelar;
2. O sistema redireciona o usuário de volta à página que solicitou a ação.

<a name='fluxos1'></a>
#### 1.6 Fluxos de Evento

##### 1.6.1 Fluxo Básico

1. O sistema gera uma janela suspensa com um formulário de cadastramento;

2. O sistema mostra três campos de inserção e uma caixa de seleção;

3. O estudante seleciona uma opção na caixa de seleção "Projeto";

4. O estudante preenche o campo "Nome" com o nome do grupo;

5. O estudante preenche o campo "Descrição" com uma breve descrição do grupo e sua finalidade;

6. O estudante preenche na seção "Membros" o usuário do membro e seleciona se o membro é ou não um administrador;

7. O sistema gera uma prévia do conteúdo e mostra ao estudante;

8. O estudante pressiona o botão "Confirmar" na aba "Visualizar".


##### 1.6.2 Fluxos Alternativos 

###### 1.6.2.1  Adicionar Membro

A qualquer momento do fluxo básico:

1. O estudante pressiona o botão "+" na aba "Cadastrar Grupo" na seção "Membros";
2. O sistema cria mais um campo de inserção, uma caixa de seleção e um botão de remoção;
3. Fim do fluxo alternativo.

Retorna ao passo 6 do fluxo básico.

###### 1.6.2.2 Remover membro

Após o passo 6 do fluxo básico:

1. O estudante pressiona o botão "x" na aba "Cadastrar Atividade" na seção "Membros";

2. O sistema remove o campo de inserção e a caixa de seleção aos quais o botão de remoção era ligado;

3. Fim do fluxo alternativo.

Retorna ao passo 7 do fluxo básico.

##### 1.6.3 Fluxos de Exceção

###### 1.6.3.1 Campo em Branco

Após o passo 8 do fluxo básico:

1. O sistema informa que há um campo de inserção ou caixa de seleção em branco;
2. Fim do fluxo exceção.

Retorna ao passo 7 do fluxo básico.

###### 1.6.3.2 Usuário inexistente

Após o passo 6 do fluxo básico:

1. O sistema informa que o usuário informado é inexistente;
2. Fim do fluxo exceção.

Retorna ao passo 6 do fluxo básico.

<a name='proto1'></a>

#### 1.7 Protótipos de Interface do Caso de Uso

##### 1.7.1 Projeto

![Protótipo de Cadastrar Projeto](https://raw.githubusercontent.com/rickyalbuq/Gametask/master/docs/prototypes/Cadastrar%20Projeto.png)

##### 1.7.2 Grupo

![Protótipo de Cadastrar Projeto - 1](https://raw.githubusercontent.com/rickyalbuq/Gametask/master/docs/prototypes/Cadastrar%20Projeto%20–%201.png)

##### 1.7.3 Outros

![Protótipo de Cadastrar Projeto - 1](https://raw.githubusercontent.com/rickyalbuq/Gametask/master/docs/prototypes/Cadastrar%20Projeto%20–%202.png)

------

<a name='visualizar'></a>

### 2 Visualizar Grupo

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

O usuário visualiza seu(s) grupo(s) já cadastrado(s).



<a name='atores2'></a>

#### 2.2 Atores

1. Estudante.

   

<a name='pre2'></a>

#### 2.3 Precondições

#####  2.3.1 Acesso à página

O usuário deve ter acesso aos links que trazem à página de visualização.

##### 2.3.2  Ter Grupos

O usuário necessita ter grupo(s) cadastrado(s).



<a name='pos2'></a>

#### 2.4 Pós-condições

##### 2.4.1 Visualização

O usuário visualiza o grupo selecionado.



<a name='ext2'></a>

#### 2.5 Pontos de Extensão

##### 2.5.1 Encerrar Grupo

Após o passo 2 do fluxo básico:

1. O estudante seleciona o seu perfil na aba "Membros";
2. O sistema gera uma janela flutuante com um botão "Sair do Grupo";
3. O estudante pressiona o botão;
4. "Encerrar Grupo".

##### 2.5.2 Mudar de Página

A qualquer momento no fluxo básico:

1. Executa-se o CDUX "Mudar Página".

##### 2.5.3 Visualizar Atividades

Após o passo 3 do fluxo básico:

1. O estudante seleciona a atividade desejada na aba "Detalhes" na sessão "Atividades";
2. Executa-se o CDUX "Visualizar Atividades".

##### 2.5.4 Visualizar Log de Atividade

Após o passo 2 do fluxo básico:

1. ???


<a name='fluxos2'></a>

#### 2.6 Fluxos de Evento

##### 2.6.1 Fluxo Básico

1. O sistema lista os grupos que o estudante tem acesso;
2. O estudante seleciona o grupo que quer visualizar;
3. O sistema retorna as infromações referentes ao grupo selecionado.
   

##### 2.6.2 Fluxos Alternativos 

###### 2.6.2.1 Criar Novo

A qualquer momento no fluxo básico:

1. O estudante pressiona o botão "Criar novo";
2. Executa-se o CDUX "Cadastrar Grupo";
3. Fim do fluxo alternativo.

Retorna ao passo 3 do fluxo básico.

###### 2.6.2.2 Editar Projeto

Após o passo 3 do fluxo básico:

1. O estudante pressiona o botão "Editar" na aba "Detalhes";
2. Executa-se o CDUX "Editar Grupo";
3. Fim do fluxo alternativo.

Retorna ao passo 3 do fluxo básico.

###### 2.6.2.3 Concluir Atividade

Após o passo 3 do fluxo básico:

1. O estudante marca a caixa de seleção da atividade desejada na aba "Detalhes";
2. Executa-se o CDUX "Concluir Atividade";
3. Fim do fluxo alternativo.

Retorna ao passo 3 do fluxo básico.



##### 2.6.3 Fluxos de Exceção

Sem Fluxos de Exceção.


<a name='proto2'></a>

#### 2.7 Protótipos de Interface do Caso de Uso

##### 

![Protótipo de Projetos](https://raw.githubusercontent.com/rickyalbuq/Gametask/master/docs/prototypes/Projetos.png)

------

<a name='editar'></a>

### 3 Editar Grupo

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

O usuário deseja editar informações de um grupo.



<a name='atores3'></a>

#### 3.2 Atores

1. Estudante.

   

<a name='pre3'></a>

#### 3.3 Precondições

#####  3.3.1 Acesso à página

O usuário deve ter acesso aos links que trazem à página de Edição.

##### 3.3.2  Ter Projetos

O usuário necessita ter grupo(s) cadastrado(s).



<a name='pos3'></a>

#### 3.4 Pós-condições

##### 3.4.1 Visualização

1. O sistema editar as informações alteradas;
2. Executa-se o CDUX "Visualizar Grupo".



<a name='ext3'></a>

#### 3.5 Pontos de Extensão


<a name='fluxos3'></a>

#### 3.6 Fluxos de Evento

##### 3.6.1 Fluxo Básico

1. Executa-se o CDUX "Visualizar Grupo"

2. O estudante selecionar a opção de editar informações do grupo;

3. O sistema mostra três campos editaveis referentes ao grupo selecionado;

4. O estudante realiza as modificações necessárias;

5. O sistema gera uma prévia do conteúdo e mostra ao estudante;

6. O estudante pressiona o botão "Confirmar";

7. O sistema retorna uma mensagem de feedback de operação realizada com sucesso.

   

##### 3.6.2 Fluxos Alternativos 

##### 3.6.2.1 Operação Cancelada

1. O estudante pressiona o botão cancelar;
2. O sistema redireciona o usuário de volta à página que solicitou a ação.

##### 3.6.3 Fluxos de Exceção

###### 3.6.3.1 Campo em Branco

Após o passo 6 do fluxo básico:

1. O sistema informa que há um campo de inserção ou caixa de seleção em branco;
2. Fim do fluxo exceção.

Retorna ao passo 4 do fluxo básico.

<a name='proto3'></a>

#### 3.7 Protótipos de Interface do Caso de Uso

##### 3.7.1 Projeto

![Protótipo de Cadastrar Projeto](https://raw.githubusercontent.com/rickyalbuq/Gametask/master/docs/prototypes/Cadastrar%20Projeto.png)

------

<a name='concluir'></a>

### 4 Concluir Grupo

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

O usuário conclui um grupo.



<a name='atores4'></a>

#### 4.2 Atores

1. Estudante.

   

<a name='pre4'></a>

#### 4.3 Precondições

#####  4.3.1 Acesso à página

O usuário deve ter acesso aos links que trazem à página de visualização.

##### 4.3.2  Ter Projetos

O usuário necessita ter grupo(s) cadastrado(s).



<a name='pos4'></a>

#### 4.4 Pós-condições

##### 4.4.1 Visualização

O usuário visualiza o grupo selecionado.



<a name='ext4'></a>

#### 4.5 Pontos de Extensão

Sem pontos de extensão.


<a name='fluxos4'></a>

#### 4.6 Fluxos de Evento

##### 4.6.1 Fluxo Básico

1. Executa-se o CDUX "Visualizar Grupo";
2. O estudante seleciona a opção "Concluir grupo";
3. O sistema pede uma confirmação ao estudante;
4. O estudante confirma a solicitação de conclusão de grupo;
5. O sistema envia um feedback informando que a operação ocorreu com sucesso.


##### 4.6.2 Fluxos Alternativos 

###### 4.6.2.1 Atividades Pendentes

Após o passo 2 do fluxo básico:

1. O sistema retorna outro pop-up avisando que existem atividades pendentes no grupo;
2. O estudante pressiona o botão "Ok";
3. O sistema retorna ao fluxo básico no passo 4


##### 4.6.3 Fluxos de Exceção

Sem Fluxos de Exceção.


<a name='proto4'></a>

#### 4.7 Protótipos de Interface do Caso de Uso

##### Visualizar

![Protótipo de Projetos](https://raw.githubusercontent.com/rickyalbuq/Gametask/master/docs/prototypes/Projetos.png)