## 1. Decisões Projetuais

### 1.1 Tecnologias

#### 1.1.1 Front-End:

-   React JS
-   Bootstrap 4
-   Sass

#### 1.1.2 Back-End:

-   Node JS
-   REST
-   Mongo DB

#### 1.1.3 Banco de Dados:

-   Decidir modelo de lista de amigos (array ou tabela)
-   Tabela única para atividades com referência em tag
-   Grupo tem tag do usuário
-   Tag em formato de matrícula

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

### 1.3 Desenvolvimento

#### 1.3.1 Método:

Descrever os métodos de desenvolvimento...

Nota: Toda sexta depois da aula (18:15)

#### 1.3.2 Escala:

| Contribuintes                     | Total de horas Semanais |
| --------------------------------- | :---------------------: |
| Arthur Meireles da Silva          |           10h           |
| Breno Pereira Alves               |           15h           |
| Euller Henrique F. de Albuquerque |           15h           |
| Jonathan Cardoso F. de Moura      |           15h           |
| Jonatas Melo Silva                |           15h           |

#### 1.3.3 Iterações

| Iteração |    Período    |                                                            Atividade                                                             |
| :------: | :-----------: | :------------------------------------------------------------------------------------------------------------------------------: |
| Primeira | 10/02 a 14/02 | Produção e Validação de Casos de Uso / Produção e Validação de Protótipos de Tela / Revisão e Apresentação das Regras de Negócio |
| Segunda  |       -       |                                                                -                                                                 |
| Terceira |       -       |                                                                -                                                                 |
|  Quarta  |       -       |                                                                -                                                                 |
|  Quinta  |       -       |                                                                -                                                                 |
|  Sexta   |       -       |                                                                -                                                                 |
|  Quinta  |       -       |                                                                -                                                                 |

#### 1.3.4 Atribuições

##### 1.3.4.1 Primeira Iteração

| Contribuintes               | Descrição                                    | Concluído |
| --------------------------- | -------------------------------------------- | :-------: |
| Arthur Meireles da Silva    | Produção dos Casos de uso UC02 e UC03        |     -     |
| Breno Pereira Alves         | Produção dos Casos de uso UC05, UC06 e UC07  |     -     |
| Euller H. F. de Albuquerque | Produção e Validação dos Protótipos de Tela  |     -     |
| Jonatas Melo Silva          | Revisão e Apresentação das Regras de Negócio |     -     |
| Jonathan C. F. de Moura     | Produção dos Casos de uso UC01 e UC04        |     -     |
