# Representação da Arquitetura

## Modelo de Arquitetura

O modelo de arquitetura adotado para este projeto foi o MVC.
A Model consiste nos dados da aplicação, regras de negócios, lógica e funções. Possibilita o reaproveitamento de código e otimização do tempo de desenvolvimento.
A View trata de exibir a aparência ou estrutura que o usuário verá na tela. É por onde o usuário irá realizar as entradas e obterá os resultados da aplicação, ou seja, irá interagir com a aplicação.
A Controller fará a mediação das entradas, convertendo-as em comandos para a Model ou para a View.

![Preview](/images/arquitecture/arq002.png?raw=true "Figura ARQ002 — Estrutura MVC")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura ARQ002 — Estrutura MVC]</h5>

## Representação do Banco de Dados - Collections
Para persistência dos dados foi utilizado o serviço Cloud Firestore do google firebase. segundo FIREBASE, 2018:

> O Cloud Firestore é um banco de dados NoSQL orientado a documentos. Ao contrário de um banco de dados SQL, não há tabelas nem linhas. Em vez disso, os dados são armazenados em documentos, que são organizados em coleções.

> Cada documento contém um conjunto de pares chave-valor. O Cloud Firestore é otimizado para armazenar grandes coleções de documentos pequenos.

>É necessário que todos os documentos sejam armazenados em coleções. Os documentos podem conter subcoleções e objetos aninhados, que podem incluir campos primitivos, como strings, ou objetos complexos, como listas.


Os esquemas apresentados abaixo têm o objetivo de ilustrar o relacionamento dos objetos no banco de dados. Todas as coleções estão aninhadas dentro da collection lista. A base de dados é composta basicamente por dois documentos raízes: O documento "User" que é responsável por armazenar os dados do usuário. E o documento "lista", responsável por armazenar todos os dados das listas de amigo secreto. Este por sua vez, possui diversas collections aninhadas, conforme podemos visualizar abaixo:

A figura COL001 demonstra a coleção responsável por armazenar os dados dos usuários cadastrados. Esta mesma estrutura é utilizada em outras Collections, conforme será apresentado mais abaixo.

![Preview](/images/collection/COL001.png?raw=true "Figura COL001 — Collection User")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura COL001 — Collection User]</h5>

A figura COL002 ilustra a coleção responsável por armazenar os dados das listas de amigo secreto criadas. Ela também é responsável por encapsular as coleções de mensagens, sugestões de presentes e o sorteio da lista.

![Preview](/images/collection/COL002.png?raw=true "Figura COL002 — Collection User")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura Collection Lista de Amigo Secreto]</h5>


A figura COL003 demonstra a estrutura de dados do autor da lista. Ela é composta exatamente pela collection da figura COL001, pois o autor é sempre um "User". Representa o usuário que criou a lista de amigo secreto.

![Preview](/images/collection/COL003.png?raw=true "Figura COL003 — Collection User")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura Subcollection lista_autor]</h5>


Na figura COL004 é definida a estrutura de dados dos participantes da lista. Ela armazena uma lista da collection "User", pois uma lista deve possuir vários participantes. Representa os participantes da lista.

![Preview](/images/collection/COL004.png?raw=true "Figura COL004 — Collection User")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura Subcollection lista_participantes]</h5>


A figura COL005 ilustra a estrutura de dados das preferências de presentes. Ela armazena uma lista da collection "User", pois assim como a lista de amigo secreto, cada preferência de presente possui um autor/dono.

![Preview](/images/collection/COL005.png?raw=true "Figura COL005 — Collection User")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura Subcollection lista_presentes]</h5>


A estrutura de dados responsável por armazenar os dados do sorteio é composta por duas subcollections de "User":
sorteio_doador e sorteio_receptor. Dentro dessas estruturas são armazenadas uma lista de usuários que participam da lista e que darão e receberão os presentes, respectivamente, conforme pode ser observado na figura COL006.

![Preview](/images/collection/COL006.png?raw=true "Figura COL006 — Collection User")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura Subcollection lista_presentes]</h5>


## Modelagem Funcional
Para o desenvolvimento deste projeto, foram construídos os seguintes artefatos de modelagem funcional:

### Estórias de Usuários
Para melhor ilustrar a solução proposta, foram criadas as estórias de usuários
listadas abaixo.

A Figura US001 ilustra a necessidade de um usuário criar uma lista de amigo secreto.

![Preview](/images/user-estory/US001.png?raw=true "Figura US001 — Cadastro de Listas de Amigo Secreto")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura US001 — Cadastro de Listas de Amigo Secreto]</h5>


A Figura US002 ilustra a necessidade de convidar os participantes da lista de amigo secreto.

![Preview](/images/user-estory/US002.png?raw=true "Figura US002 — Convidar participantes para a lista")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura US002 — Convidar participantes para a lista]</h5>


Na figura US003 é demonstrada a necessidade de cadastrar as preferências de presentes dos participantes.

![Preview](/images/user-estory/US003.png?raw=true "Figura US003 — Cadastrar preferências de presentes")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura US003 — Cadastrar preferências de presentes]</h5>


Na figura US004 ilustra a necessidade do usuário visualizar o seu amigo secreto sorteado, ao qual deverá presentear.

![Preview](/images/user-estory/US004.png?raw=true "Figura US004 — Visualizar Amigo Secreto Sorteado")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura US004 — Enviar mensagens aos participantes]</h5>


A figura US005 especifica a necessidade dos usuários de realizar o sorteio da lista de amigo secreto para que os participantes saibam à quem deverão presentear.

![Preview](/images/user-estory/US005.png?raw=true "Figura US005 — Realizar sorteio da lista")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura US005 — Realizar sorteio da lista]</h5>


A necessidade de manter atualizados os participantes da lista através de “push notifications” está descrita na figura US006.

![Preview](/images/user-estory/US006.png?raw=true "Figura US006 — Receber Notificações Push aos Participantes")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura US006 — Receber Notificações Push aos Participantes]</h5>


Na figura US007 o usuário descreve a necessidade de realizar seu cadastro na aplicação para ter acesso aos seus dados.
![Preview](/images/user-estory/US007.png?raw=true "Figura US007 — Cadastrar Perfil")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura US007 — Cadastrar Perfil]</h5>


A Figura US008 ilustra a necessidade do usuário utilizar a área de login para realizar o acesso às informações do app Meu Amigo Secreto, gerenciar as informações das suas listas de amigo secreto ou as listas das quais participa.

![Preview](/images/user-estory/US008.png?raw=true "Figura US008 — Realizar Login")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura US008 — Realizar Login]</h5>


Na figura US009 o usuário descreve a necessidade de atualizar as suas informações de perfil de usuário.

![Preview](/images/user-estory/US009.png?raw=true "Figura US009 — Visualizar e Editar Perfil")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura US009 — Visualizar e Editar Perfil]</h5>


A figura US010 é descrita a necessidade dos usuários de trocar mensagens com os participantes da lista de amigo secreto a qual fazem parte.

![Preview](/images/user-estory/US010.png?raw=true "Figura US010 — Visualizar Amigo Secreto Sorteado")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura US010 — Enviar mensagens aos participantes]</h5>


### Product Backlog
Abaixo segue o Product Backlog do projeto App MAS - Meu Amigo Secreto. Nele é possível verificar a distribuição das tarefas e suas prioridades de execução.

![Preview](/images/backlog/back001.png?raw=true "Figura BACK001 — Product Backlog")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura BACK001 — Product Backlog]</h5>

### Backlog Item
Abaixo segue o Backlog Item do projeto App MAS - Meu Amigo Secreto. Nele é possível verificar a distribuição das tarefas nas Sprints.

[colocar imagem do backlog item]
![Preview](/images/backlog/back001.png?raw=true "Figura BACK001 — Product Backlog")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura BACK001 — Product Backlog]</h5>

### Wireframes
Abaixo, seguem os wireframes do projeto, utilizados para criação da interface gráfica do projeto. Estes wireframes foram utilizados como base para a criação das telas da aplicação.

#### Interface da listagem de amigo secreto
![Preview](/images/wireframe/WIR001.png?raw=true "Figura WIR001 — Tela com as Listas de Amigo Secreto do MAS")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura BACK001 — Listas de Amigo Secreto]</h5>



#### Interface do Profile do usuário
![Preview](/images/wireframe/WIR002.png?raw=true "Figura WIR002 — Tela de Profile do MAS")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura WIR002 — Profile]</h5>


#### Interface da Interação de usuários via mensagens
![Preview](/images/wireframe/WIR003.png?raw=true "Figura WIR003 — Tela de troca de mensagens entre usuários do MAS")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura WIR003 — Lista de mensagens trocadas entre usuários do MAS]</h5>


#### Interface da listagem de mensagens trocadas
![Preview](/images/wireframe/WIR004.png?raw=true "Figura WIR004 — Listagem com as mensagens trocadas entre usuários do MAS")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura WIR004 — Lista de mensagens]</h5>


#### Interface da listagem das preferências de presentes
![Preview](/images/wireframe/WIR005.png?raw=true "Figura WIR005 — Listagem com as preferências de presentes dos usuários do MAS")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura WIR003 — Lista com as preferências de presentes]</h5>
