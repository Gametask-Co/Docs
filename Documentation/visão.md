# Documento de visão - Gametask

## 1. Introdução

### 1.1 Resumo

O Gametask consiste em uma solução integradora de gestão de tempo e atividades acadêmicas voltado para estudantes (secundaristas, acadêmicos e vestibulandos).

O sistema se propõe a solucionar a fragmentação de múltiplas aplicações voltadas para estudo, aprimoramento de aptidão dos usuários em gerenciar sua rotina e tempo, melhoramento de métodos de organização, aperfeiçoamento de disciplina e assiduidade e produção de cronogramas bem definidos para aumento de entusiasmo através de metas acessíveis.

A ferramenta possibilita uma gestão integradora de atividades e rotinas, que através da ludificação mantém níveis saudáveis de estímulo sobre as tarefas e objetivos que ao serem realizadas em tempo determinado concedem recompensas de experiência e hierarquia no ambiente interativo da aplicação.

### 1.2 Escopo

Tendo em vista o propósito do projeto (gerenciar rotinas e atividades acadêmicas) seguem abaixo as principais responsabilidades e não-responsabilidades do sistema.

#### 1.2.1 Responsabilidades do Sistema

1. Permitir a criação, acompanhamento e gerenciamento de atividades;
2. Permitir a criação, acompanhamento e gerenciamento de disciplinas;
3. Permitir a criação, acompanhamento e gerenciamento de projetos;
4. Gerar esquemas de horário e rotina baseado em informações fornecidas pelo usuário;
5. Auxiliar na gestão do tempo escolar;
6. Recompensar a realização de tarefas através da ludificação.

#### 1.2.2 Não-Responsabilidades do Sistema

1. Guardar documentos, imagens, áudios ou vídeos;
2. Criar ou editar documentos, imagens, áudios ou vídeos;
3. Enviar, receber ou anexar arquivos;
4. Permitir o recebimento ou emissão de notas para atividades por terceiros;
5. Intermediar estudantes e educadores;
6. Gerir funções escolares;
7. Permitir troca de mensagens;
8. Permitir o acompanhamento das atividades de outrem.

## 2. Requisitos

### 2.1 Requisitos Funcionais

| Cód. | Nome                            | Descrição                                                    | Prioridade |
| :--: | :------------------------------ | ------------------------------------------------------------ | :--------: |
| RF01 | Criação de Conta                     | O usuário poderá criar uma conta                             |    Alta    |
| RF02 | Autenticação de Usuários                      | O usuário poderá autenticar-se utilizando uma conta preexistente |    Alta    |
| RF03 | Exclusão de Contas                   | O usuário poderá excluir sua conta                           |   Média    |
| RF04 | Edição de Conta                    | O usuário poderá editar informações da conta                 |   Média    |
| RF05 | Adição de Atividade             | O usuário poderá criar uma atividade                         |    Alta    |
| RF06 | Edição Atividade                | O usuário poderá alterar a atividade                         |   Média    |
| RF07 | Cancelamento de Atividade              | O usuário poderá cancelar a atividade                        |    Alta    |
| RF08 | Visualização de Atividade            | O usuário poderá visualizar a atividade                      |    Alta    |
| RF09 | Conclusão de Atividade              | O usuário poderá concluir a atividade                        |    Alta    |
| RF10 | Adição de Disciplina            | O usuário poderá criar uma disciplina                        |    Alta    |
| RF11 | Edição de Disciplina               | O usuário poderá alterar a disciplina                        |   Média    |
| RF12 | Cancelamento de Disciplina             | O usuário poderá cancelar a disciplina                       |   Média    |
| RF13 | Visualização de Disciplina           | O usuário poderá visualizar a disciplina                     |    Alta    |
| RF14 | Conclusão de Disciplina             | O sistema concluirá a disciplina na data informada           |   Média    |
| RF15 | Adição de Projeto               | O usuário poderá criar um projeto                            |    Alta    |
| RF16 | Edição de Projeto                  | O usuário poderá alterar o projeto                           |   Média    |
| RF17 | Cancelamento de Projeto                | O usuário poderá cancelar o projeto                          |   Média    |
| RF18 | Visualização de Projeto              | O usuário poderá visualizar o projeto                        |    Alta    |
| RF19 | Conclusão de Projeto                | O usuário poderá concluir o projeto                          |   Média    |
| RF20 | Adição de Grupo                 | O usuário poderá criar um grupo                              |    Alta    |
| RF21 | Edição de Grupo                    | O usuário poderá alterar um grupo                            |   Média    |
| RF22 | Exclusão de  Grupo                   | O usuário poderá excluir um grupo                            |   Baixa    |
| RF23 | Visualização de Grupo                | O usuário poderá visualizar o grupo selecionado              |    Alta    |
| RF24 | Adição de Integrante            | O usuário poderá adicionar um usuário ao grupo               |    Alta    |
| RF25 | Remoção de Integrante              | O usuário poderá remover um integrante do grupo              |   Baixa    |
| RF26 | Visualização de Usuário              | O usuário poderá visualizar o perfil de outro usuário        |   Médio    |
| RF27 | Adição Administrador         | O usuário poderá adicionar um integrante do grupo como administrador |   Baixa    |
| RF28 | Visualização de Linha do Tempo       | O usuário poderá visualizar a linha do tempo (calendário e horários) na dashboard |   Média    |
| RF29 | Adição à Lista de Tarefas    | O usuário poderá adicionar tarefas à lista de tarefas referente a uma atividade |   Média    |
| RF30 | Adição à Lista de Atividades | O usuário poderá adicionar atividades à lista de atividades referente a um projeto ou grupo |   Média    |
| RF31 | Delegação de Atividade               | O usuário poderá delegar uma tarefa a um integrante do grupo |    Alta    |
| RF32 | Visualização de Fluxo                | O usuário poderá visualizar o log de interações do grupo     |   Baixa    |
| RF33 | Adição de Amigo                 | O usuário pode enviar um pedido de amizade a outro usuário   |   Baixa    |
| RF34 | Busca de Usuário                  | O usuário pode buscar outro usuário na plataforma            |   Baixa    |
| RF35 | Pontuação do Usuário                 | Ao concluir uma atividade o Sistema dá pontos ao usuário     |   Média    |

### 2.2 Requisitos Não-Funcionais

| Cód. | Nome                    | Descrição                                                    | Categoria   |
| ---- | ----------------------- | ------------------------------------------------------------ | ----------- |
| NF01 | Ludificação             | Ganhos e perdas adquiridos através da realização de objetivos. | Obrigatório |
| NF02 | Segurança               | Tráfego seguro das informações pessoais de tarefas e integrações realizadas. | Desejável   |
| NF03 | Desempenho              | Utilização de boas práticas para o uso de dados leves e otimizados. | Desejável   |
| NF04 | Usabilidade             | Uso de linguagem facilitada dos componentes e partes importantes do sistema. | Obrigatório |
| NF05 | Portabilidade           | Fácil exportação dos dados do sistema para outras tecnologias podendo ser feito também integrações | Obrigatório |
| NF06 | Parâmetros anti-trapaça | Prevenção contra jogadores trapaceiros                       | Obrigatório |

### 2.3 Tabela de Referência - Requisitos

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

### 2.4 Diagrama Geral de Casos de Uso



### 2.5 Casos de Uso

| Cód. | Caso de Uso            | Descrição                                                    | Classificação |
| ---- | ---------------------- | ------------------------------------------------------------ | ------------- |
| UC01 | Gerenciar Usuários     | Cadastrar, editar, visualizar e deletar um usuário           | Primário      |
| UC02 | Gerenciar Atividades   | Cadastrar, editar, visualizar e deletar uma atividade        | Primário      |
| UC03 | Gerenciar Disciplinas  | Cadastrar, editar, visualizar e deletar uma disciplina       | Primário      |
| UC04 | Gerenciar Projetos     | Cadastrar, editar, visualizar e deletar um projeto           | Primário      |
| UC05 | Gerenciar Grupo        | Criar,visualizar e excluir um grupo                          | Primário      |
| UC06 | Gerenciar Integrantes  | Inserir e remover integrantes de um grupo, dar e remover privilégios | Secundário    |
| UC07 | Transferência de dados | Importar ou exportados do/para o Gametask                    | Secundário    |

### 2.6 Tabela de Referência - Casos de uso & Requisitos

|      | UC01 | UC02 | UC03 | UC04 | UC05 | UC06 | UC07 |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| RF01 |  X   |      |      |      |      |      |      |
| RF02 |  X   |      |      |      |      |      |      |
| RF03 |  X   |      |      |      |      |      |      |
| RF04 |  X   |      |      |      |      |      |      |
| RF05 |      |  X   |      |      |      |      |      |
| RF06 |      |  X   |      |      |      |      |      |
| RF07 |      |  X   |      |      |      |      |      |
| RF08 |      |  X   |      |      |      |      |      |
| RF09 |      |  X   |      |      |      |      |      |
| RF10 |      |      |  X   |      |      |      |      |
| RF11 |      |      |  X   |      |      |      |      |
| RF12 |      |  X   |  X   |      |      |      |      |
| RF13 |      |  X   |  X   |      |      |      |      |
| RF14 |      |      |  X   |      |      |      |      |
| RF15 |      |      |      |  X   |      |      |      |
| RF16 |      |  X   |      |  X   |      |      |      |
| RF17 |      |  X   |      |  X   |      |      |      |
| RF18 |      |      |      |  X   |      |      |      |
| RF19 |      |      |      |  X   |      |      |      |
| RF20 |      |      |      |      |  X   |      |      |
| RF21 |      |      |      |      |  X   |      |      |
| RF22 |      |  X   |      |  X   |  X   |      |      |
| RF23 |      |      |      |      |  X   |      |      |
| RF24 |      |      |      |      |      |  X   |      |
| RF25 |      |      |      |      |      |  X   |      |
| RF26 |  X   |      |      |      |      |  X   |      |
| RF27 |      |      |      |      |      |  X   |      |
| RF28 |      |      |      |      |  X   |      |      |
| RF29 |      |  X   |      |      |      |      |      |
| RF30 |      |  X   |      |  X   |  X   |      |      |
| RF31 |      |      |      |      |  X   |      |      |
| RF32 |      |      |      |      |  X   |      |      |
| RF33 |  X   |      |      |      |      |      |      |
| RF34 |  X   |      |      |      |      |      |      |
| RF35 |      |  X   |      |      |      |      |      |

### 2.7 Atores

| Ator      | Descrição                                                    |
| --------- | ------------------------------------------------------------ |
| Estudante | Jovens e adultos de segmento secundarista, vestibulando e universitário |
| Sistema   | Referente ao servidor que mantem a API interna               |
| Serviço   | Referente a um servidor externo que mantem uma API de serviços integrada ao sistema |

## 3. Restrições

| Cód. | Nome                     | Descrição                                               | Categoria   |
| ---- | ------------------------ | ------------------------------------------------------- | ----------- |
| R01  | Acesso à internet        | Necessário para conseguir a autenticação da conta       | Obrigatório |
| R02  | Estar Autenticado        | Necessário para conseguir visualizar os dados da conta  | Obrigatório |
| R03  | Cadastrar Dados Pessoais | Cadastrar dados pessoais para interagir com a aplicação | Obrigatório |
| R04  | Cadastrar Atividade      | Cadastrar atividade para interagir com a aplicação      | Desejável   |
| R05  | Cadastrar Projeto        | Cadastrar projeto para interagir com a aplicação        | Desejável   |
| R06  | Cadastrar Disciplina     | Cadastrar disciplina para interagir com a aplicação     | Desejável   |

## 4. Riscos

| Descrição                     | Impacto                                               |
| ------------------------ | ------------------------------------------------------- |
| Mudança de tecnologia      | Alto       |
| Saída de integrantes        | Médio  |
| Falta de recursos para hospedagem | Médio |
| Falta de recursos para implementação      | Alto      |

## 5. Stackholders

### 5.1 Clientes

Universidades, escolas e instituições de ensino que queiram estimular seus estudantes a tornar suas rotinas de estudo mais produtivas. E estudantes que por conta própria desejem o auxilio de uma ferramenta de produtividade em nicho especifico.

### 5.2 Usuários

Estudantes secundaristas, acadêmicos e vestibulandos.

## 6. Diagramas

### 6.1 Diagrama de Casos de Uso

![Diagrama de casos de uso](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Documentation/Diagramas/UC%20Diagram%20-%20Gametask.png)

### 6.2 Diagrama de Classes

![Diagrama de classes](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Documentation/Diagramas/Class%20Diagram%20-%20Gametask.png)



## 7. API



[Documentação](https://gametask.docs.apiary.io/)

