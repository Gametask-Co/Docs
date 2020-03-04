# Documento de Projeto



## 1. Decisões

### 1.1 Tecnologias

#### 1.1.1 Front-End:

-   React JS
-   Sass

#### 1.1.2 Back-End:

-   Node JS
-   REST
-   Mongo DB

### 1.2 Regras de Negócio

#### 1.2.1 Sistema de pontuação

|        Peso         | Min. | Méd. | Max. |
| :-----------------: | :--: | :--: | :--: |
| Número de Afazeres  |  0   |  -   |  10  |
| Estado da Atividade |  0   | 0.5  |  1   |
|     Prazo Final     |  0   | 0.25 |  1   |

#### 1.2.2 Cálculo:

```python
#Calculo Base da Pontuação
def calc_point(n_todo=0, state=0.5, due_date=0.25, todo_const=10):
    value = todo_const * n_todo
    if value > 100:
        value = 100

    return value * state * due_date
```

#### 1.2.3 Ludificação

Aqui vai o que Jonatas pesquisou...



## 2. Desenvolvimento

#### 2.1 Método:

Descrever os métodos de desenvolvimento...

Nota: Toda sexta depois da aula (18:15)

#### 2.2 Escala:

| Contribuintes                     | Total de horas Semanais |
| --------------------------------- | :---------------------: |
| Arthur Meireles da Silva          |           10h           |
| Breno Pereira Alves               |           15h           |
| Euller Henrique F. de Albuquerque |           15h           |
| Jonathan Cardoso F. de Moura      |           15h           |
| Jonatas Melo Silva                |           15h           |

#### 2.3 Iterações

| Iteração |    Período    |                          Atividade                           |
| :------: | :-----------: | :----------------------------------------------------------: |
| Primeira | 10/02 a 14/02 | Produção e Validação de Casos de Uso / Produção e Validação de Protótipos de Tela / Revisão e Apresentação das Regras de Negócio |
| Segunda  | 17/02 a 28/02 | Revisão de Documentos / Construção de Issues / Produção de documentação da API / Revisão de Diagramas |
| Terceira | 02/03 a 13/03 | Validação da Arquitetura / Construção de Estruturas e Rotas para 'Tasks' / Implementação da Interface para os casos de uso de 'Tasks' |
|  Quarta  | 16/03 a 27/03 | Construção de Estruturas e Rotas para 'Project' / Implementação da Interface para os casos de uso de 'Project' |
|  Quinta  | 30/03 a 10/04 | Construção de Estruturas e Rotas para 'Subject' / Implementação da Interface para os casos de uso de 'Subject' |
|  Sexta   | 13/04 a 24/04 | Construção de Estruturas e Rotas para 'Group' / Implementação da Interface para os casos de uso de 'Group' |
|  Sétima  | 27/04 a 08/05 | Construção de Estruturas e Rotas para Integrações / Implementação da Interface para as partes de Ludifacação e Ranking |
|  Oitava  | 11/05 a 22/05 | Transicionar a aplicação / Realizar testes com usuários / Revisar documentação |

#### 2.4 Atribuições

##### 2.4.1 Primeira Iteração (10/02 a 14/02)

| Contribuintes               | Descrição                                    | Concluído |
| --------------------------- | -------------------------------------------- | :-------: |
| Arthur Meireles da Silva    | Produção dos Casos de uso UC02 e UC03        |    OK     |
| Breno Pereira Alves         | Produção dos Casos de uso UC05, UC06 e UC07  |    OK     |
| Euller H. F. de Albuquerque | Produção e Validação dos Protótipos de Tela  |    OK     |
| Jonatas Melo Silva          | Revisão e Apresentação das Regras de Negócio |     -     |
| Jonathan C. F. de Moura     | Produção dos Casos de uso UC01 e UC04        |    OK     |

##### 2.4.2 Segunda Iteração (17/02 a 28/02)

| Contribuintes               | Descrição                                       | Concluído |
| --------------------------- | ----------------------------------------------- | :-------: |
| Arthur Meireles da Silva    | Revisão de Diagramas - CDUs e Classes           |    OK     |
| Breno Pereira Alves         | Documentação da API                             |    OK     |
| Euller H. F. de Albuquerque | Construção das Issues                           |     -     |
| Jonatas Melo Silva          | Ausente                                         |     -     |
| Jonathan C. F. de Moura     | Construção do Glossário e das Regras de Negócio |    OK     |

##### 2.4.3 Terceira Iteração (02/03 a 13/03)

| Contribuintes               | Descrição                                                   | Concluído |
| --------------------------- | ----------------------------------------------------------- | :-------: |
| Arthur Meireles da Silva    | Construção de Módulo de Tela - Task                         |     -     |
| Breno Pereira Alves         | Finalização de modulo de API - Task                         |     -     |
| Euller H. F. de Albuquerque | Finalizar revisões de Documentação                          |     -     |
| Jonatas Melo Silva          | Construção de roteiro e implementação de teste de interface |     -     |
| Jonathan C. F. de Moura     | Construção de módulos de Modais e Mensagens                 |     -     |

##### 2.4.4 Quarta Iteração (16/03 a 27/03)

| Contribuintes               | Descrição | Concluído |
| --------------------------- | --------- | :-------: |
| Arthur Meireles da Silva    | -         |     -     |
| Breno Pereira Alves         | -         |     -     |
| Euller H. F. de Albuquerque | -         |     -     |
| Jonatas Melo Silva          | -         |     -     |
| Jonathan C. F. de Moura     | -         |     -     |

##### 2.4.5 Quinta Iteração (30/03 a 10/04)

| Contribuintes               | Descrição | Concluído |
| --------------------------- | --------- | :-------: |
| Arthur Meireles da Silva    | -         |     -     |
| Breno Pereira Alves         | -         |     -     |
| Euller H. F. de Albuquerque | -         |     -     |
| Jonatas Melo Silva          | -         |     -     |
| Jonathan C. F. de Moura     | -         |     -     |

##### 2.4.6 Sexta Iteração (13/04 a 24/04)

| Contribuintes               | Descrição | Concluído |
| --------------------------- | --------- | :-------: |
| Arthur Meireles da Silva    | -         |     -     |
| Breno Pereira Alves         | -         |     -     |
| Euller H. F. de Albuquerque | -         |     -     |
| Jonatas Melo Silva          | -         |     -     |
|  Jonathan C. F. de Moura     | - |     -     |

##### 2.4.7 Quinta Iteração (27/04 a 08/05)

| Contribuintes               | Descrição | Concluído |
| --------------------------- | --------- | :-------: |
| Arthur Meireles da Silva    | -         |     -     |
| Breno Pereira Alves         | -         |     -     |
| Euller H. F. de Albuquerque | -         |     -     |
| Jonatas Melo Silva          | -         |     -     |
| Jonathan C. F. de Moura     | -         |     -     |

##### 2.4.8 Sexta Iteração (11/05 a 22/05)

| Contribuintes               | Descrição | Concluído |
| --------------------------- | --------- | :-------: |
| Arthur Meireles da Silva    | -         |     -     |
| Breno Pereira Alves         | -         |     -     |
| Euller H. F. de Albuquerque | -         |     -     |
| Jonatas Melo Silva          | -         |     -     |
| Jonathan C. F. de Moura     | -         |     -     |