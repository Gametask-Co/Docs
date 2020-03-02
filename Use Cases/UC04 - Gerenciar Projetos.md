# Especificação de Caso de Uso Gametask

## CDU04 - Gerenciar Projeto

| Índice Geral                      |
| :-------------------------------- |
| [Cadastrar Projeto](#cadastro)    |
| [Visualizar Projeto](#visualizar) |
| [Editar Projeto](#editar)         |
| [Concluir Projeto](#concluir)     |

------

<a name='cadastro'></a>

### 1 Cadastrar Projeto

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

O usuário cadastra um novo projeto em sua conta.



<a name='atores1'></a>

#### 1.2 Atores

1. Estudante.

   

<a name='pre1'></a>

#### 1.3 Precondições

#####  1.3.1 Está Autenticado

O usuário deve está autenticado em sua conta para efetuar o cadastramento.

#####  1.3.2 Acesso à página

O usuário deve ter acesso aos links que trazem a página de cadastramento.



<a name='pos1'></a>

#### 1.4 Pós-condições

##### 1.4.1 Cadastro Efetuado

1. O sistema salva as informações inseridas e cadastra um novo projeto;

2. O sistema redireciona o usuário de volta à pagina que solicitou a ação.

   

<a name='ext1'></a>

#### 1.5 Pontos de Extensão

##### 1.5.1 Cadastrar Tarefa

1. Após o cadastramento de um novo projeto o usuário está habilitado a cadastrar novas atividades relacionadas aquele projeto;

2. O sistema redireciona o usuário para o caso de uso UC02 - Gerenciar Atividades.



<a name='fluxos1'></a>
#### 1.6 Fluxos de Evento

##### 1.6.1 Fluxo Básico

1. O sistema gera uma janela suspensa com um formulário de cadastramento;

2. O sistema pré-seleciona a opção "Avulso" na aba "Modelos";

3. O sistema mostra três campos de inserção e uma caixa de seleção;

4. O estudante seleciona uma opção na caixa de seleção "Projeto";

5. O estudante preenche o campo "Prazo" com a data final do projeto;

6. O estudante preenche o campo "Nome" com o que identifique o projeto;

7. O estudante preenche o campo "Descrição" com uma breve descrição do projeto;

8. O sistema gera uma prévia do conteúdo e mostra ao estudante;

9. O estudante pressiona o botão "Confirmar" na aba "Visualizar".

   

##### 1.6.2 Fluxos Alternativos 

###### 1.6.2.1  Modelo Grupo

A qualquer momento do fluxo básico:

1. O estudante pressiona o botão "Grupo" na aba "Modelos";
2. O sistema mostra três campos de inserção e uma caixa de seleção;
3. O estudante seleciona uma opção na caixa de seleção "Grupo";
4. Fim do fluxo alternativo.

Retorna ao passo 4 do fluxo básico.

###### 1.6.2.2 Modelo Outros

A qualquer momento do fluxo básico:

1. O estudante pressiona o botão "Outros" na aba "Modelos";
2. O sistema mostra três campos de inserção;
3. Fim do fluxo alternativo.

Retorna ao passo 4 do fluxo básico.



##### 1.6.3 Fluxos de Exceção

###### 1.6.3.1 Campo em Branco

Após o passo 8 do fluxo básico:

1. O sistema informa que há um campo de inserção ou caixa de seleção em branco;
2. Fim do fluxo exceção.

Retorna ao passo 7 do fluxo básico.

###### 1.6.3.2 Prazo Inválido

Após o passo 8 do fluxo básico:

1. O sistema informa que o prazo informado é inválido;
2. Fim do fluxo exceção.

Retorna ao passo 4 do fluxo básico.



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

### 2 Visualizar Projeto

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

O usuário visualiza seus projetos já cadastrados.



<a name='atores2'></a>

#### 2.2 Atores

1. Estudante.

   

<a name='pre2'></a>

#### 2.3 Precondições

#####  2.3.1 Acesso à página

O usuário deve ter acesso aos links que trazem à página de visualização.

##### 2.3.2  Ter Projetos

O usuário necessita ter projetos cadastrados.



<a name='pos2'></a>

#### 2.4 Pós-condições

##### 2.4.1 Visualização

O usuário visualiza o projeto selecionado.



<a name='ext2'></a>

#### 2.5 Pontos de Extensão

##### 2.5.1 Concluir Projeto

Após o passo 3 do fluxo básico:

1. O estudante pressiona o botão "Concluir" na aba "Detalhes";

2. Executa-se o UC04 - Gerenciar Projeto.

   

<a name='fluxos2'></a>

#### 2.6 Fluxos de Evento

##### 2.6.1 Fluxo Básico

2. O estudante seleciona na aba "Resultados" o projeto desejado;

3. O sistema preenche com as informações referentes ao projeto escolhido a aba "Detalhes".

   

##### 2.6.2 Fluxos Alternativos 

###### 2.6.2.1  Ver Outros Projetos

A qualquer momento no fluxo básico:

1. O estudante seleciona na aba "Resultados" outro projeto desejado;
2. Fim do fluxo alternativo.

Retorna ao passo 2 do fluxo básico.

###### 2.6.2.3 Editar Projeto

Após o passo 2 do fluxo básico:

1. O estudante pressiona o botão "Editar" na aba "Detalhes";
2. Executa-se o UC04 - Gerênciar Projeto;
3. Fim do fluxo alternativo.

Retorna ao passo 2 do fluxo básico.



##### 2.6.3 Fluxos de Exceção

Sem Fluxos de Exceção.



<a name='proto2'></a>

#### 2.7 Protótipos de Interface do Caso de Uso

![Protótipo de Projetos](https://raw.githubusercontent.com/rickyalbuq/Gametask/master/docs/prototypes/Projetos.png)

------

<a name='editar'></a>

### 3 Editar Projeto

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

O usuário deseja editar informações relacionadas a um projeto cadastrado.



<a name='atores3'></a>

#### 3.2 Atores

1. Estudante.

   

<a name='pre3'></a>

#### 3.3 Precondições

#####  3.3.1 Acesso à página

O usuário deve ter acesso aos links que trazem à página de Edição.

##### 3.3.2  Ter Projetos

O usuário necessita ter projetos cadastrados.



<a name='pos3'></a>

#### 3.4 Pós-condições

##### 3.4.1 Visualização

1. O sistema editar as informações alteradas;
2. Executa-se o UC04 - Gerenciar Projetos.



<a name='ext3'></a>

#### 3.5 Pontos de Extensão

Não há pontos de extensão.



<a name='fluxos3'></a>

#### 3.6 Fluxos de Evento

##### 3.6.1 Fluxo Básico

1. O estudante seleciona o card do projeto na seção de "Resultados";

2. O sistema mostra três campos de inserção e uma caixa de seleção;

3. O estudante preenche o campo "Prazo" com a data final do projeto;

4. O estudante preenche o campo "Nome" com o que identifique o projeto;

5. O estudante seleciona uma opção na caixa de seleção "Disciplina";

6. O estudante preenche o campo "Descrição" com uma breve descrição do projeto;

8. O estudante pressiona o botão "Confirmar".

   

##### 3.6.2 Fluxos Alternativos 

Não há fluxos alternativos.



##### 3.6.3 Fluxos de Exceção

###### 3.6.3.1 Prazo Inválido

Após o passo 7 do fluxo básico:

1. O sistema informa que o prazo informado é inválido;
2. Fim do fluxo exceção.

Retorna ao passo 3 do fluxo básico.



<a name='proto3'></a>

#### 3.7 Protótipos de Interface do Caso de Uso

##### 3.7.1 Projeto

![Protótipo de Cadastrar Projeto](https://raw.githubusercontent.com/rickyalbuq/Gametask/master/docs/prototypes/Cadastrar%20Projeto.png)

------

<a name='concluir'></a>

### 4 Concluir Projeto

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

O usuário deseja concluir um projeto.



<a name='atores4'></a>

#### 4.2 Atores

1. Estudante.

   

<a name='pre4'></a>

#### 4.3 Precondições

#####  4.3.1 Acesso à página

O usuário deve ter acesso aos links que trazem à página de visualização.

##### 4.3.2  Ter Projetos

O usuário necessita ter projetos cadastrados.



<a name='pos4'></a>

#### 4.4 Pós-condições

##### 4.4.1 Visualização

O usuário visualiza o projeto selecionado.



<a name='ext4'></a>

#### 4.5 Pontos de Extensão

Não há pontos de extensão.



<a name='fluxos4'></a>

#### 4.6 Fluxos de Evento

##### 4.6.1 Fluxo Básico

1. O estudante pressiona o botão "Concluir" na aba "Detalhes" do projeto selecionado;

2. O sistema retorna um pop-up pedindo confirmação para conclusão do projeto;

3. O estudante pressiona o botão "Confirmar";

4. O sistema salva o projeto com o status de concluído e atribui pontos ao estudante pela conclusão;

5. O sistema retorna uma mensagem que o projeto foi concluído com sucesso;

6. O sistema retorna  para a tela de visualização de projetos.

   

##### 4.6.2 Fluxos Alternativos 

###### 4.6.2.1 Atividades Pendentes

Após o passo 3 do fluxo básico:

1. O sistema retorna outro pop-up avisando que existem atividades pendentes no projeto;
2. O estudante pressiona o botão "Ok";
3. O sistema retorna para a tela de "Visualizar Projetos".



##### 4.6.3 Fluxos de Exceção

Sem Fluxos de Exceção.



<a name='proto4'></a>

#### 4.7 Protótipos de Interface do Caso de Uso

##### Visualizar

![Protótipo de Projetos](https://raw.githubusercontent.com/rickyalbuq/Gametask/master/docs/prototypes/Projetos.png)



