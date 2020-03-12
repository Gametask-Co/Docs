# Gametask
## Documento de Arquitetura de Sistema



|    Data    | Versão |                  Descrição                   |         Autor          |
| :--------: | :----: | :------------------------------------------: | :--------------------: |
| 09/05/2020 |  1.0   | Adição dos Diagramas de Contexto e Container | Euller H F Albuquerque |



## 1 Arquitetura

#### 1.1 Visão do ambiente computacional e físico

##### 1.1.1 Diagrama de Contexto

![Diagrama de Contexto](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Documentation/Diagramas/Context%20Diagram.png)

##### 1.1.2 Diagrama de Container

![Diagrama de Container](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Documentation/Diagramas/Container%20Diagram.png)

##### 1.1.3 Requisitos Significativos para a Arquitetura

###### 1.1.3.1 Requisitos Funcionais

| Cód. | Nome                            | Descrição                                                    | Prioridade |
| :--: | :------------------------------ | ------------------------------------------------------------ | :--------: |
| RF01 | Criar Conta                     | O usuário poderá criar uma conta                             |    Alta    |
| RF02 | Autenticar                      | O usuário poderá autenticar-se utilizando uma conta preexistente |    Alta    |
| RF03 | Excluir Conta                   | O usuário poderá excluir sua conta                           |   Média    |
| RF04 | Editar Conta                    | O usuário poderá editar informações da conta                 |   Média    |
| RF05 | Adicionar Atividade             | O usuário poderá criar uma atividade                         |    Alta    |
| RF06 | Editar Atividade                | O usuário poderá alterar a atividade                         |   Média    |
| RF07 | Cancelar Atividade              | O usuário poderá cancelar a atividade                        |    Alta    |
| RF08 | Visualizar Atividade            | O usuário poderá visualizar a atividade                      |    Alta    |
| RF09 | Concluir Atividade              | O usuário poderá concluir a atividade                        |    Alta    |
| RF10 | Adicionar Disciplina            | O usuário poderá criar uma disciplina                        |    Alta    |
| RF11 | Editar Disciplina               | O usuário poderá alterar a disciplina                        |   Média    |
| RF12 | Cancelar Disciplina             | O usuário poderá cancelar a disciplina                       |   Média    |
| RF13 | Visualizar Disciplina           | O usuário poderá visualizar a disciplina                     |    Alta    |
| RF14 | Concluir Disciplina             | O sistema concluirá a disciplina na data informada           |   Média    |
| RF15 | Adicionar Projeto               | O usuário poderá criar um projeto                            |    Alta    |
| RF16 | Editar Projeto                  | O usuário poderá alterar o projeto                           |   Média    |
| RF17 | Cancelar Projeto                | O usuário poderá cancelar o projeto                          |   Média    |
| RF18 | Visualizar Projeto              | O usuário poderá visualizar o projeto                        |    Alta    |
| RF19 | Concluir Projeto                | O usuário poderá concluir o projeto                          |   Média    |
| RF20 | Adicionar Grupo                 | O usuário poderá criar um grupo                              |    Alta    |
| RF21 | Editar Grupo                    | O usuário poderá alterar um grupo                            |   Média    |
| RF22 | Excluir Grupo                   | O usuário poderá excluir um grupo                            |   Baixa    |
| RF23 | Visualizar Grupo                | O usuário poderá visualizar o grupo selecionado              |    Alta    |
| RF24 | Adicionar Integrante            | O usuário poderá adicionar um usuário ao grupo               |    Alta    |
| RF25 | Remover Integrante              | O usuário poderá remover um integrante do grupo              |   Baixa    |
| RF26 | Visualizar Usuário              | O usuário poderá visualizar o perfil de outro usuário        |   Médio    |
| RF27 | Adicionar Administrador         | O usuário poderá adicionar um integrante do grupo como administrador |   Baixa    |
| RF28 | Visualizar Linha do Tempo       | O usuário poderá visualizar a linha do tempo (calendário e horários) na dashboard |   Média    |
| RF29 | Adicionar à Lista de Tarefas    | O usuário poderá adicionar tarefas à lista de tarefas referente a uma atividade |   Média    |
| RF30 | Adicionar à Lista de Atividades | O usuário poderá adicionar atividades à lista de atividades referente a um projeto ou grupo |   Média    |
| RF31 | Delegar Atividade               | O usuário poderá delegar uma tarefa a um integrante do grupo |    Alta    |
| RF32 | Visualizar Fluxo                | O usuário poderá visualizar o log de interações do grupo     |   Baixa    |
| RF33 | Adicionar Amigo                 | O usuário pode enviar um pedido de amizade a outro usuário   |   Baixa    |
| RF34 | Buscar Usuário                  | O usuário pode buscar outro usuário na plataforma            |   Baixa    |
| RF35 | Pontuar Usuário                 | Ao concluir uma atividade o Sistema dá pontos ao usuário     |   Média    |

###### 1.1.3.2 Requisitos Não-Funcionais

| Cód. | Nome                    | Descrição                                                    | Categoria   |
| ---- | ----------------------- | ------------------------------------------------------------ | ----------- |
| NF01 | Ludificação             | Ganhos e perdas adquiridos através da realização de objetivos. | Obrigatório |
| NF02 | Segurança               | Tráfego seguro das informações pessoais de tarefas e integrações realizadas. | Desejável   |
| NF03 | Desempenho              | Utilização de boas práticas para o uso de dados leves e otimizados. | Desejável   |
| NF04 | Usabilidade             | Uso de linguagem facilitada dos componentes e partes importantes do sistema. | Obrigatório |
| NF05 | Portabilidade           | Fácil exportação dos dados do sistema para outras tecnologias podendo ser feito também integrações | Obrigatório |
| NF06 | Parâmetros anti-trapaça | Prevenção contra jogadores trapaceiros                       | Obrigatório |

###### 1.1.3.3 Tabela de Referência - Requisitos

|      | NF01 | NF02 | NF03 | NF04 | NF05 | NF06 |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| RF01 |      |  X   |  X   |  X   |      |      |
| RF02 |      |  X   |  X   |  X   |      |      |
| RF03 |      |  X   |  X   |  X   |      |      |
| RF04 |      |  X   |  X   |  X   |      |      |
| RF05 |      |  X   |  X   |  X   |  X   |      |
| RF06 |      |      |  X   |  X   |  X   |      |
| RF07 |      |      |  X   |  X   |  X   |      |
| RF08 |      |  X   |  X   |  X   |  X   |      |
| RF09 |  X   |      |  X   |  X   |  X   |      |
| RF10 |      |  X   |  X   |  X   |  X   |      |
| RF11 |      |      |  X   |  X   |  X   |      |
| RF12 |      |      |  X   |  X   |  X   |      |
| RF13 |      |  X   |  X   |  X   |  X   |      |
| RF14 |  X   |      |  X   |  X   |  X   |      |
| RF15 |      |  X   |  X   |  X   |  X   |      |
| RF16 |      |      |  X   |  X   |  X   |      |
| RF17 |      |      |  X   |  X   |  X   |      |
| RF18 |      |  X   |  X   |  X   |  X   |      |
| RF19 |  X   |      |  X   |  X   |  X   |      |
| RF20 |      |  X   |  X   |  X   |      |      |
| RF21 |      |      |  X   |  X   |      |      |
| RF22 |      |      |  X   |  X   |      |      |
| RF23 |      |  X   |  X   |  X   |      |      |
| RF24 |      |      |  X   |  X   |      |      |
| RF25 |      |      |  X   |  X   |      |      |
| RF26 |      |  X   |  X   |  X   |      |      |
| RF27 |      |      |  X   |  X   |      |      |
| RF28 |      |      |  X   |  X   |      |      |
| RF29 |      |  X   |  X   |  X   |  X   |      |
| RF30 |      |  X   |  X   |  X   |  X   |      |
| RF31 |      |      |  X   |  X   |      |      |
| RF32 |      |  X   |  X   |  X   |      |      |
| RF33 |      |  X   |  X   |  X   |      |      |
| RF34 |      |      |  X   |  X   |      |      |
| RF35 |  X   |      |  X   |  X   |      |  X   |


#### 1.2 Visão macro dos pacotes ou sub-sistemas

A definir.

## 2 Estilo Arquitetural

#### 2.1 Descrição do Estilo Arquitetural

A definir.

## 3 Pacotes ou Sub-Sistemas

#### 3.1 Pacote de interface com o usuário

A definir.

#### 3.2 Pacote de negócio (serviços do sistema)

A definir.

#### 3.3 Pacote de persistência

A definir.

#### 3.4 Subsistema de mensagens assíncronas

A definir.

## 4 Anexos

A definir.