# Especificação de Caso de Uso Gametask

## CDU01 - Gerenciar Usuário

| Índice Geral                      |
| :-------------------------------- |
| [Cadastrar Usuário](#cadastro)    |
| [Visualizar Usuário](#visualizar) |
| [Editar Usuário](#editar)         |
| [Excluir Usuário](#Excluir)       |

------

<a name='cadastro'></a>

### 1 Cadastrar Usuário

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

O estudante cadastra-se na plataforma Gametask.



<a name='atores1'></a>

#### 1.2 Atores

1. Estudante;

2. Serviços (Google e Facebook).

   

<a name='pre1'></a>

#### 1.3 Precondições

#####  1.3.1 Acesso à página

O estudante deve acessar a página inicial da aplicação e clicar em algum dos links e botões de cadastro.



<a name='pos1'></a>

#### 1.4 Pós-condições

##### 1.4.1 Cadastro Efetuado

1. O sistema salva as informações inseridas e cadastra o novo usuário;
2. O estudante é redirecionado para um tutorial na página de dashboard.



<a name='ext1'></a>

#### 1.5 Pontos de Extensão

#### 1.5.1 Usuário já cadastrado

A qualquer momento no fluxo básico:

1. O estudante pressiona o link "Já tem uma conta? Entre";
2. O sistema redireciona o usuário de volta à página de autenticação.



<a name='fluxos1'></a>

#### 1.6 Fluxos de Evento

##### 1.6.1 Fluxo Básico

2. O sistema mostra na primeira de quatro páginas, três campos de inserção;

3. O estudante preenche o campo "E-mail" com um e-mail válido;

5. O estudante preenche o campo "Senha" com uma senha válida;

6. O estudante preenche o campo "Confirmar Senha" com a mesma senha digitada no campo de "Senha";

8. O estudante pressiona o botão "Cadastrar";

9. O estudante é redirecionado para a segunda página de cadastro;

7. O sistema apresenta três campos de inserção, uma caixa de seleção e um botão para upload de foto;

8. O estudante preenche o campo "Nome" com seu primeiro nome;

9. O estudante preenche o campo "Sobrenome" com o ultimo sobrenome;

10. O estudante preenche o campo "Nascimento" com a sua data de nascimento;

11. O estudante seleciona no campo "Gênero" o gênero que melhor lhe corresponde;

12. O estudante pressiona o botão "Alterar" no campo "Avatar";

13. O sistema faz uma chamada de sistema para o explorador de arquivos do usuário;

14. O estudante seleciona uma imagem válida;

15. O sistema carrega uma previa da imagem;

16. O estudante confirma o upload da imagem clicando no botão "Confirmar";

17. O estudante pressiona o botão "Continuar";

18. O estudante é redirecionado para a terceira página de cadastro;

19. O sistema gera dois botões radiais, "Casual" e "Competitivo";

20. O estudante seleciona o modo de jogo que mais lhe agrada e pressiona o botão "Continuar"; 

21. O estudante é redirecionado para a quarta e ultima página de cadastro;

22. O sistema gera seis botões radiais, cada um com uma cor diferente;

23. O estudante seleciona uma cor;

24. O sistema mostra uma previa do sistema na cor escolhida;

25. O estudante pressiona o botão "Concluir";

    

##### 1.6.2 Fluxos Alternativos 

###### 1.6.2.1 Autenticação com conta Google

Antes do passo 5 do fluxo básico:

1. O estudante pressiona o botão "Entrar com Google";
2. O serviço abre uma nova janela com a tela de autenticação Google;
3. O estudante segue os passos indicados pelo serviço e fecha a janela;
4. O sistema recebe as informações do Serviço e preenche de maneira previa os campos da segunda pagina de cadastro;
5. Fim do fluxo exceção.

Retorna ao passo 6 do fluxo básico.

###### 1.6.2.2 Autenticação com conta Facebook

Antes do passo 5 do fluxo básico:

1. O estudante pressiona o botão "Continue com Facebook";
2. O serviço abre uma nova janela com a tela de autenticação Facebook;
3. O estudante segue os passos indicados pelo serviço e fecha a janela;
4. O sistema recebe as informações do Serviço e preenche de maneira previa os campos da segunda pagina de cadastro;
5. Fim do fluxo exceção.

Retorna ao passo 6 do fluxo básico.



##### 1.6.3 Fluxos de Exceção

###### 1.6.3.1 Campo em Branco

A qualquer momento do fluxo básico:

1. O sistema informa que há um campo de inserção, botão radial ou caixa de seleção em branco;
2. Fim do fluxo exceção.

Retorna ao passo anterior ao erro.

###### 1.6.3.2 E-mail Inválido

Após o passo 5 do fluxo básico:

1. O sistema informa que o e-mail informado é inválido;
2. Fim do fluxo exceção.

Retorna ao passo 2 do fluxo básico.

##### 1.6.3.3 Senha Inválida

Após o passo 5 do fluxo básico:

1. O sistema informa que a senha informada é inválida;
2. Fim do fluxo exceção.

Retorna ao passo 3 do fluxo básico.

##### 1.6.3.4 Senhas Incompatíveis

Após o passo 5 do fluxo básico:

1. O sistema informa que as senhas informadas não são compatíveis;
2. Fim do fluxo exceção.

Retorna ao passo 4 do fluxo básico.

##### 1.6.3.5 Imagem Inválida

Após o passo 16 do fluxo básico:

1. O sistema informa que a imagem enviada é inválida;
2. Fim do fluxo exceção.

Retorna ao passo 12 do fluxo básico.

##### 1.6.3.6 Limite de caracteres excedido

A qualquer momento do fluxo básico:

1. O sistema informa que o limite de caracteres do campo foi excedido;
2. Fim do fluxo exceção.

Retorna ao passo anterior ao erro.



<a name='proto1'></a>

#### 1.7 Protótipos de Interface do Caso de Uso

##### 1.7.1 Primeira página

![Protótipo de Cadastrar Usuário - 1](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Sign%20In.png)

##### 1.7.2 Segunda página

![Protótipo de Cadastrar Usuário - 2](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Complete%20Profile.png)

##### 1.7.3 Terceira página

![Protótipo de Cadastrar Usuário - 3](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Type%20of%20Gamification.png)

##### 1.7.3 Quarta página

![Protótipo de Cadastrar Usuário - 4](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Color%20Picker.png)

------

<a name='visualizar'></a>

### 2 Visualizar Usuário

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

O estudante visualiza o perfil de outros usuários já cadastrados na plataforma.



<a name='atores2'></a>

#### 2.2 Atores

1. Estudante.

   

<a name='pre2'></a>

#### 2.3 Precondições

#####  2.3.1 Está autenticado

O estudante deve está autenticado para buscar usuários cadastrados.

##### 2.3.2  Informar usuário

O estudante necessita informar o nome ou e-mail de um usuário cadastrado.



<a name='pos2'></a>

#### 2.4 Pós-condições

##### 2.4.1 Visualização

O usuário visualiza o perfil do usuário selecionado.



<a name='ext2'></a>

#### 2.5 Pontos de Extensão

##### 2.5.1 Adicionar usuário

A definir.

##### 2.5.2 Bloquear usuário

A definir.

<a name='fluxos2'></a>

#### 2.6 Fluxos de Evento

##### 2.6.1 Fluxo Básico

1. O estudante seleciona no menu lateral o ícone com sua foto;
2. O estudante seleciona "Amigos" na seção Perfil;
3. O sistema preenche a tela com as informações referentes aos perfis já conhecidos e com uma caixa de pesquisa;
4. O estudante clica em um perfil;
5. O sistema gera uma janela flutuante com as informações do perfil selecionado.



##### 2.6.2 Fluxos Alternativos 

###### 2.6.2.1  Buscar usuário

Após o passo 3 do fluxo básico:

1. O estudante digita o nome ou e-mail de um usuário;
2. O sistema devolve todas as opções que satisfazem a busca;
3. Fim do fluxo alternativo.

Retorna ao passo 4 do fluxo básico.



##### 2.6.3 Fluxos de Exceção

###### 2.6.3.1  Usuário não encontrado

Após o passo 1 do fluxo alternativo "Buscar Usuário":

1. O sistema informa que não há opções que satisfaçam a busca;
2. Fim do fluxo exceção.

Retorna ao passo 1 do fluxo alternativo "Buscar Usuário".

###### 2.6.3.2 Busca em Branco

Após o passo 1 do fluxo alternativo "Buscar Usuário":

1. O sistema informa que o campo de busca está em branco;
2. Fim do fluxo exceção.

Retorna ao passo 1 do fluxo alternativo "Buscar Usuário".

###### 2.6.3.3 E-mail Inválido

Após o passo 1 do fluxo alternativo "Buscar Usuário":

1. O sistema informa que o e-mail informado é inválido;
2. Fim do fluxo exceção.

Retorna ao passo 1 do fluxo alternativo "Buscar Usuário".



<a name='proto2'></a>

#### 2.7 Protótipos de Interface do Caso de Uso

![Protótipo de visualizar usuários](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

------

<a name='editar'></a>

### 3 Editar Usuário

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

O estudante edita informações relacionadas ao seu próprio perfil.



<a name='atores3'></a>

#### 3.2 Atores

1. Estudante.

   

<a name='pre3'></a>

#### 3.3 Precondições

#####  3.3.1 Está autenticado

O estudante deve está autenticado para editar seu perfil.



<a name='pos3'></a>

#### 3.4 Pós-condições

##### 3.4.1 Cadastro

1. O sistema salva as informações inseridas no perfil do usuário;
2. O sistema redireciona o usuário cadastrado para a página de dashboard.



<a name='ext3'></a>

#### 3.5 Pontos de Extensão

Não há fluxos de extensão.



<a name='fluxos3'></a>

#### 3.6 Fluxos de Evento

##### 3.6.1 Fluxo Básico

1. O estudante seleciona no menu lateral o ícone com sua foto;

2. O estudante seleciona "Editar" na seção Perfil;

3. O sistema apresenta dois campos de inserção, uma caixa de seleção e um botão para upload de foto;

4. O estudante preenche o campo "Nome" com seu primeiro nome;

5. O estudante preenche o campo "Sobrenome" com o ultimo sobrenome;

6. O estudante seleciona no campo "Gênero" o gênero que melhor lhe corresponde;

7. O estudante pressiona o botão "Alterar" no campo "Avatar";

8. O sistema faz uma chamada de sistema para o explorador de arquivos do usuário;

9. O estudante seleciona uma imagem válida;

10. O sistema carrega uma previa da imagem;

11. O estudante confirma o upload da imagem clicando no botão "Confirmar";

12. O estudante pressiona o botão "Salvar";

13. O sistema solicita a senha do usuário em uma janela flutuante;

14. O estudante fornece a senha correta e pressiona o botão "Confirmar";

15. O sistema informa que as alterações foram salvas com sucesso;

    

#### 3.6.2 Fluxos Alternativos 

Não há fluxos alternativos.



#### 3.6.3 Fluxos de Exceção

###### 3.6.3.1 Campo em Branco

Após o passo 12 do fluxo básico:

1. O sistema informa que há um campo de inserção, botão radial ou caixa de seleção em branco;
2. Fim do fluxo exceção.

Retorna ao passo anterior ao erro.

##### 3.6.3.2 Senha Inválida

Após o passo 14 do fluxo básico:

1. O sistema informa que a senha informada é inválida;
2. Fim do fluxo exceção.

Retorna ao passo 13 do fluxo básico.

##### 3.6.3.3 Imagem Inválida

Após o passo 11 do fluxo básico:

1. O sistema informa que a imagem enviada é inválida;
2. Fim do fluxo exceção.

Retorna ao passo 7 do fluxo básico.

##### 3.6.3.4 Limite de caracteres excedido

A qualquer momento do fluxo básico:

1. O sistema informa que o limite de caracteres do campo foi excedido;
2. Fim do fluxo exceção.

Retorna ao passo anterior ao erro.



<a name='proto3'></a>

#### 3.7 Protótipos de Interface do Caso de Uso

##### 3.7.1 Usuário

![Protótipo de Editar Usuário](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)

------

<a name='Excluir'></a>

### 4 Excluir Usuário

| Índice Excluir                |
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

O estudante desativa seu próprio perfil.



<a name='atores4'></a>

#### 4.2 Atores

1. Estudante.

   

<a name='pre4'></a>

#### 4.3 Precondições

#####  4.3.1 Está autenticado

O estudante deve está autenticado para desativar seu perfil.



<a name='pos4'></a>

#### 4.4 Pós-condições

##### 4.4.1 Visualização

1. O sistema confirma que o usuário foi desativado;

2. O sistema redireciona o usuário a pagina de autenticação.

   

<a name='ext4'></a>

#### 4.5 Pontos de Extensão

Não há fluxos de extensão.



<a name='fluxos4'></a>

#### 4.6 Fluxos de Evento

##### 4.6.1 Fluxo Básico

1. O estudante seleciona no menu lateral o ícone "Configurações";

2. O estudante seleciona "Desativar Conta" na aba lateral;

3. O sistema gera uma janela flutuante solicitando a senha do usuário para confirmar a operação;

4. O estudante fornece a senha correta e pressiona o botão "Confirmar";

5. O sistema informa que as alterações foram salvas com sucesso;

   

##### 4.6.2 Fluxos Alternativos 

Não há fluxos alternativos.



##### 4.6.3 Fluxos de Exceção

##### 4.6.3.1 Senha Inválida

Após o passo 4 do fluxo básico:

1. O sistema informa que a senha informada é inválida;
2. Fim do fluxo exceção.

Retorna ao passo 3 do fluxo básico.



<a name='proto4'></a>

#### 4.7 Protótipos de Interface do Caso de Uso

##### Visualizar

![Protótipo de Deletar Usuário](https://raw.githubusercontent.com/Gametask-Co/GT-DOCS/master/Prototypes/Working.png)



