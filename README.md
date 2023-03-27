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
* **O empréstimo de livros com no mínimo X de participantes de um grupo;**
* **A estilização do site é muito antiga e pré histórica;**

Como os empréstimos são feitos apenas em grupos, não há localização de onde se encontra meus livros.
Nossos empréstimos não funcionarão apenas tendo uma lista definida de participantes em nosso grupos disponibilizados e também teremos nossas exigências em relação aos empréstimos.
A estilização do site é muito antiga, não chamando atenção para novos usuários. 




# Descrição da proposta

O acesso total do site será feito pelos administradores, enquanto os usuários terão um acesso um pouco restritivo ao site. Para o cadastro de usuários serão solicitados dados básicos como login, email e senha possibilitando assim a criação de sua conta no site. Os usuários terão acesso para o cadastro de livros que será feito por categorias que já estão armazenadas em nosso banco de dados e pelo ISBN do livro, caso o ISBN cadastrado já exista não será permitido novamente o cadastro desse livro. Não haverá um cadastro das categorias pelos usuários, nosso sistema já fornecerá as categorias existentes.

O nosso sistema de empréstimo será feito somente por livros físicos, em que quando um usuário emprestar seu livro, ele poderá cadastrar que foi realizado o empréstimo listando categorias, nome do livro, tempo de empréstimo e email do usuário a quem foi emprestado. O controle de devolução é por conta do usuário. 


Relatórios? 
**

# Regras de Negócio