## Representação do Banco de Dados - Collections

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
