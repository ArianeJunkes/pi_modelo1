# Projeto Integrador - Daarii

Projeto Integrador do Curso de Técnico em Desenvolvimento de Sistemas para a Internet Integrado ao Ensino Médio do IFC - Campus Araquari.

Alunos: [Davi Gabriel Tomaz](https://github.com/davigtomaz) e [Ariane Tainara Junkes](https://github.com/ArianeJunkes).

Links do projeto:

-   [Documentação (esse documento)](github.com/marcoandre/pi-modelo)
-   [Backend](github.com/marcoandre/pi-backend)
-   [Frontend](github.com/marcoandre/pi-frontend)

# Situação Problema

[Skoob](http://www.skoob.com.br/)
    
A empresa escolhida foi o Skoob, existente desde 2009, criado pelo brasileiro Lindenberg Moreira, associado com a Viviane Lordello profissional de Marketing. Contando com mais de 8.2 milhões de usuários cadastrados no site. Através de cadastro, é possível listar o que você está lendo, o que já leu, o que pretende ler, o que está relendo e quais leituras foram abandonadas, formando assim uma "estante" virtual. O sistema tem um "paginômetro", que soma as páginas dos livros marcados como já lidos, além de uma média de páginas. Títulos ainda ausentes no banco de dados podem ser adicionados pelos próprios usuários, que podem compartilhar suas opiniões sobre as obras através de avaliações com estrelas, de uma a cinco, e resenhas. Possui também a opção de participar de grupos com temas diversos, desde Livros Viajantes (um usuário se dispõe a emprestar um livro de acordo com a lista de participantes definida) à Colecionadores de Marcadores de Texto. Atualmente o Skoob disponibilizou gratuitamente App para iOS e Android.



## Problemas Observados 

* **Falta de localização de onde esses livros estão fisicamente;**
* **A estilização do site é muito antiga e pré histórica;**

Como os empréstimos são feitos apenas em grupos, não há localização de onde se encontra meus livros emprestados e não emprestados.
A estilização do site é muito antiga, não chamando atenção para novos usuários. 




# Descrição da proposta

O acesso total do site será feito pelos administradores, enquanto os usuários terão um acesso um pouco restritivo ao site. Para o cadastro de usuários serão solicitados dados básicos como login, email e senha possibilitando assim a criação de sua conta no site. Os usuários terão acesso para o cadastro de livros que será feito por categorias que já estão armazenadas em nosso banco de dados e pelo ISBN do livro, caso o ISBN cadastrado já exista não será permitido novamente o cadastro desse livro. Não haverá um cadastro das categorias pelos usuários, nosso sistema já fornecerá as categorias existentes.

O nosso sistema de empréstimo será feito somente por livros físicos, em que quando um usuário emprestar seu livro, ele poderá cadastrar que foi realizado o empréstimo listando categorias, nome do livro, tempo de empréstimo e email do usuário a quem foi emprestado. O controle de devolução é por conta do usuário. 

Teremos relatórios gerados pelo sistema de livros lidos por ano, livros mais emprestados e menos emprestados, e relatórios de opiniões.


# Regras de Negócio

RN001- Cadastro de usuários: Os usuários precisam fazer cadastro para realizar empréstimos.

RN002- Realizar empréstimo: Para realizar o empréstimo, apenas usuários cadastro e nenhum emprétimos em aberto.

RN003- Listagem de empréstimo: O usuário precisa listar o livro que irá emprestar.

RN004- Registro de empréstimo: O administrador deve possuir acesso ao registro de empréstimo.

RN005- Devolução de empréstimo: O usuário deve registrar a devolução.

RN006- Cadastro de livros: Para usuário inserir um novo livro, precisa apenas do nome e autor, pois categorias já estão armazenadas. 

RN007- Cadastro de feedback: O usuário pode registrar um feedback sobre os livros que ele emprestou.

RN008- Registro de relatório: O administrador deve possuir acesso ao regristo de relatório.

# Requisitos Funcionais 

Entradas

R.F.01 - Cadastro de usuário: Para cadastro de usuário precisa de dados como email e a criação de uma senha. Usuário: todos os níveis de usuário.

R.F.02 - Cadastro de livros: Para cadastro de livros precisa de dados como categoria, editora e autor. Usuário: todos os níveis de usuário.

R.F.03 - Cadastro de feedback: Para cadastro de feedback precisa de dados como nome do livros, nome do usuário e comentário sobre o livro. Usuário: todos os níveis de usuário.

R.F.04 - Registro de empréstimos: Para registrar um empréstimo de livro é necessário nome do usuário, nome do livro e data de pedido. Usuário: todos os níveis de usuário.

R.F.05 - Devolução de empréstimo: Para registro de devolução de empréstimo é necessário nome de usuário, nome do livro e data da devolução. Usuário: todos os níveis de usuário.

Processos

R.F.06 - Autenticação de usuário: tem como propósito autenticar o acesso ao sistema, verificando se o usuário pode acessá-lo e, caso possa, o direcionando para a página principal de seu perfil de acesso.
Dados necessários: email, senha, nível de permissão.
Usuários: todos os níveis de usuário.

R.F.07 - Listagem de empréstimos: tem como propósito informar quantos livros o usuário tem emprestado. Usuário: todos os níveis de usuário. Usuário: todos os níveis de usuário.


Saídas


R.F.08 - Registro de relatório: Para registro de relatório precisa de dados como sobre o que será o relatório exemplo: livros mais lidos, livros mais emprestados, etc... Usuário: apenas vizualização.

# Requisitos Não Funcionais

