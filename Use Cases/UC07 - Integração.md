# Especificação de Caso de Uso Gametask

## CDU05 - Gerenciar Integração

| Índice Geral                    |
| :------------------------------ |
| [Exportar Dados](#exportar)     |
| [Importar Dados](#importar) |

------

<a name='exportar'></a>

### 1 Exportar Dados

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

O Estudante exporta os seus dados contido na plataforma Gametask.



<a name='atores1'></a>

#### 1.2 Atores

1. Estudante.

   

<a name='pre1'></a>

#### 1.3 Precondições

#####  1.3.1 Estar Autenticado

O estudante deve está autenticado em sua conta para efetuar a exportação de dados.

<a name='pos1'></a>
#### 1.4 Pós-condições

##### 1.4.1 Feedback

1. O sistema deve informar a situação do pedido de exportação de dados (em fila/concluido).

<a name='ext1'></a>
#### 1.5 Pontos de Extensão

##### 1.5.1 Operação Cancelada

1. O estudante pressiona o botão cancelar;
2. O sistema redireciona o usuário de volta à página que solicitou a ação.

<a name='fluxos1'></a>
#### 1.6 Fluxos de Evento

##### 1.6.1 Fluxo Básico

1. O sistema gera uma janela suspensa com as opções de integração;
2. O estudante escolhe a opção de exportação de dados;
3. O sistema informa que o pedido foi pra fila de processamento;
4. O sistema redireciona o estudante para a página de integração.


##### 1.6.2 Fluxos Alternativos 

Sem fluxo alternativos.


##### 1.6.3 Fluxos de Exceção

###### 1.6.3.1 Limite de pedidos

Após o passo 2 do fluxo básico:

1. O sistema informa que o estudante já fez outro pedido em menos de 2h;

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

<a name='importar'></a>

### 2 Importar Dados

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

O estudante importa dados para a plataforma Gametask


<a name='atores2'></a>

#### 2.2 Atores

1. Estudante.

   

<a name='pre2'></a>

#### 2.3 Precondições

#####  2.3.1 Estar Autenticado

O estudante deve está autenticado em sua conta para efetuar a exportação de dados.

#####  2.3.2 Informações em formato JSON

O estudante deve fornecer à plataforma um arquivo em formato JSON com a estrutura e dados coerente ao da plataforma.


<a name='pos2'></a>

#### 2.4 Pós-condições

##### 2.4.1 Feedback

1. O sistema deve informar a situação do pedido de importação de dados (em fila/concluido).

<a name='ext2'></a>

#### 2.5 Pontos de Extensão

Sem ponto de extensão.

<a name='fluxos2'></a>

#### 2.6 Fluxos de Evento

##### 2.6.1 Fluxo Básico

1. O sistema gera uma janela suspensa com as opções de integração;
2. O estudante escolhe a opção de importar de dados;
3. O sistema gera uma janela com opção para selecionar um arquivo do desktop;
4. O estudante escolhe o arquivo;
5. O estudante faz o upload do arquivo e confirma a ação;
6. O sistema informa que o pedido foi pra fila de processamento;
7. O sistema redireciona o estudante para a página de integração.


##### 2.6.2 Fluxos Alternativos 

Sem fluxo alternativos.


##### 2.6.3 Fluxos de Exceção

###### 2.6.3.1 Arquivo com extensão incorreta

Após o passo 5 do fluxo básico:

1. O sistema informa que o arquivo fornecido não está com extensão .JSON;
2. O sistema informa um link de auxílio ao estudante em como formatar de forma correta o arquivo.

Retorna ao passo 1 do fluxo básico.


<a name='proto2'></a>

#### 2.7 Protótipos de Interface do Caso de Uso

##### 

![Protótipo de Projetos](https://raw.githubusercontent.com/rickyalbuq/Gametask/master/docs/prototypes/Projetos.png)

------
