# Funcionalidades do App MAS
Abaixo seguem as funcionalidades que estão disponíveis na aplicação e as funcionalidades que serão implementadas:

## a) Gerenciamento de Listas de amigo secreto
Através desta tela é possível cadastrar as listas de amigo secreto, clicando no ícone "+", localizado no canto inferior direito.
Nesta tela serão exibidas as listas as quais o usuário faz parte ou

![Preview](images/functionality/FUN005.png?raw=true "Figura FUN005 — Cadastro de Usuário")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN005 — Recuperação de Senha]</h6>

Após isso, o usuário será direcionado para o formulário de cadastro da lista de amigo secreto, conforme demonstrado na Figura FUN006.

![Preview](images/functionality/FUN006.png?raw=true "Figura FUN006 — Cadastro de Usuário")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN006 — Cadastro de Listas de Amigo Secreto]</h6>

O usuário deverá informar o valor mínimo do presente, a data do sorteio e a data da confraternização - troca de presentes. Também será possível inserir os participantes na lista - devendo o usuário inserir-se ou não, pois ele pode criar a lista e não participar.
Para adicionar um participante à lista o administrador da lista deverá informar o nº de telefone do participante que deseja inserir. Apenas o participante que criou a lista poderá realizar alterações na mesma. Participantes da lista podem apenas visualizar os participantes da lista e as informações cadastradas pelo participante administrador.

![Preview](images/functionality/FUN007.png?raw=true "Figura FUN007 — Cadastro de Usuário")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN007 — Cadastro de Listas de Amigo Secreto]</h6>








## b) Convidar pessoas para participar da lista
Após o administrador da lista enviar o link do convite - é utilizada a própria API de envio do próprio dispositivo - as pessoas com esse link podem aceitar participar da lista ou rejeitar. Neste link terá um redirecionamento para o download do app e após a instalação e cadastro, o usuário receberá uma notificação de que foi convidado a participar da lista de amigo secreto. 
A própria API nativa do dispositivo permite o envio do convite através de Whatsapp, sms ou qualquer outro aplicativo de envio de mensagens de texto.
O convite não revela o amigo secreto dos participantes, apenas tem o intuito de facilitar a adesão à lista por parte dos participantes.

## c) Troca de informações sobre as preferências de presentes
Os participantes terão a opção de cadastrar suas sugestões de presentes. Poderão informar que presente gostaria de receber, bem como as características do mesmo. Estas informações podem ser, por exemplo, a loja onde o presente pode ser comprado; um link para compra online do produto; detalhes de tamanho e cor; e o que mais for necessário para facilitar a identificação do presente desejado.

## d) Troca de mensagens em grupo ou individualmente de forma anônima
Através da própria aplicação os participantes da lista poderão trocar mensagens com o grupo, ou seja, a lista de amigo secreto à qual fazem parte. Essas mensagens ficarão visíveis a todos os participantes da lista. Também terá a opção de troca de mensagem entre presenteados e presenteadores de forma anônima, o que garante o anonimato na brincadeira.

## e) Realização do sorteio sem que haja confusão - sortear a si próprio
O sorteio será realizado pelo administrador da lista e há garantia de que não haverá sorteios inválidos, ou seja, um participante presenteando a si próprio ou um participante sendo presenteado por mais de um participante da lista. Assim que o sorteio for realizado os participantes receberão uma notificação informando-os sobre o sorteio.
O sorteio será justo e sem trapaças, não sendo possível selecionar critérios para favorecer o sorteio. Sendo assim, o sorteio será completamente aleatório.

## f) Manter os participantes atualizados sobre as informações da lista
Para que todos os participantes saibam das alterações nas informações da lista de amigo secreto à qual fazem parte e se mantenham atualizados, sempre que alguma modificação ocorrer na lista os participantes da lista serão notificados através de push notification.

## g) Interface de cadastro de usuário
Para acessar a aplicação, todos os usuários deverão efetuar o cadastro prévio para ter acesso aos dados da lista ou para criar novas listas de amigo secreto.
Para realizar o cadastro é necessário que o usuário informe seu número de telefone com DDD, seu nome ou apelido e defina uma senha de acesso. Assim que o usuário inserir o código corretamente, ele será redirecionado para a tela principal da aplicação.
Estes dados podem ser alterados através da tela de Perfil do Usuário, caso ele necessite.

![Preview](images/functionality/FUN002.png?raw=true "Figura FUN002 — Cadastro de Usuário")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN002 — Cadastro de usuário]</h6>

## h) Interface para realizar login
Na tela de login o usuário deverá informar o número de telefone com DDD e a senha que foram cadastrados previamente. Se os dados estiverem corretos ele será redirecionado para a tela principal da aplicação. É nesta tela que eles poderão realizar o cadastro, clicando em "cadastre-se!". Também é possível redefinir a senha clicando em "Esqueceu sua senha?".

![Preview](images/functionality/FUN003.png?raw=true "Figura FUN003 — Cadastro de Usuário")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN003 — Cadastro de usuário]</h6>

Ao clicar em "Esqueceu sua senha?" será exibida uma Popup solicitando ao usuário que informe o telefone cadastrado com DDD.

![Preview](images/functionality/FUN004.png?raw=true "Figura FUN004 — Cadastro de Usuário")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN004 — Recuperação de Senha]</h6>

## i) Interface para visualizar e editar o perfil
O usuário terá uma opção para editar seus dados cadastrais. Através dessa interface será possível alterar dados como senha, nome e avatar. Não será possível alterar o número de telefone que foi cadastrado pelo usuário.
Para o avatar é definida uma imagem default do sistema. O usuário poderá alterar seu avatar uma única vez e esta alteração é realizada de forma randômica pela aplicação, ou seja, existe uma biblioteca de avatares e ao alterar o avatar o sistema automaticamente escolherá uma dessas imagens da biblioteca. Assim que essa imagem for aleatoriamente escolhida ela é salva automaticamente e o usuário não pode mais alterá-la.

## j) Visualização do respectivo amigo secreto, obtido após a realização do sorteio
Os participantes poderão visualizar quem é seu respectivo amigo secreto. Cada participante poderá visualizar o seu amigo secreto correspondente, à quem deverá presentear. 
O administrador da lista não terá, em hipótese alguma, a opção de visualizar o resultado do sorteio. Ele somente poderá ver quem é seu amigo secreto - no caso em que esteja participando da brincadeira.
