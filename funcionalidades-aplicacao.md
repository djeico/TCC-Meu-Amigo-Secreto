# Funcionalidades do App MAS
Abaixo seguem as funcionalidades que estão disponíveis na aplicação e as funcionalidades que serão implementadas:

## a) Gerenciamento de Listas de amigo secreto
Através desta tela é possível cadastrar as listas de amigo secreto, clicando no ícone "+", localizado no canto inferior direito.
Nesta tela serão exibidas as listas as quais o usuário faz parte ou

![Preview](images/functionality/FUN005.png?raw=true "Figura FUN005 — Gerenciamento das Listas de Amigo Secreto")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN005 — Gerenciamento das Listas de Amigo Secreto]</h6>

Após isso, o usuário será direcionado para o formulário de cadastro da lista de amigo secreto, conforme demonstrado na Figura FUN006.

![Preview](images/functionality/FUN006.png?raw=true "Figura FUN006 — Cadastro de Listas de Amigo Secreto")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN006 — Cadastro de Listas de Amigo Secreto]</h6>

O usuário deverá informar o valor mínimo do presente, a data do sorteio e a data da confraternização - troca de presentes. Também será possível inserir os participantes na lista - devendo o usuário inserir-se ou não, pois ele pode criar a lista e não participar.
Para adicionar um participante à lista o administrador da lista deverá informar o nº de telefone do participante que deseja inserir, conforme demonstra a Figura FUN007.

![Preview](images/functionality/FUN007.png?raw=true "Figura FUN007 — Cadastro de Listas de Amigo Secreto")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN007 — Cadastro de Listas de Amigo Secreto]</h6>

Assim que o participante for adicionado ele será relacionado logo abaixo do formulário, conforme Figura FUN010.

![Preview](images/functionality/FUN010.png?raw=true "Figura FUN010 — Adição de participantes na lista")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN010 — Adição de participantes na lista]</h6>

É possível adicionar um participante mesmo que ele ainda não tenha cadastro no App MAS. Neste caso, ele é exibido como "Aguardando Cadastro", conforme Figura FUN010. Quando ele fizer o cadastro, será exibido com os dados atualizados.
Depois de inseridos todos os dados da lista, basta clicar em salvar.

## b) Convidar pessoas para participar da lista
Após o administrador da lista enviar o link do convite - é utilizada a própria API de envio do dispositivo. As pessoas receberão um link que terá um redirecionamento para o download do App MAS e após a instalação e cadastro, o usuário receberá uma notificação de que foi convidado a participar da lista de amigo secreto. Ele poderá optar por aceitar o convite ou rejeitá-lo.
A própria API nativa do dispositivo permite o envio do convite através de Whatsapp, sms ou qualquer outro aplicativo de envio de mensagens de texto.
O convite não revela o amigo secreto dos participantes, apenas tem o intuito de facilitar o download e adesão à lista por parte dos participantes.

![Preview](images/functionality/FUN009B.png?raw=true "Figura FUN009 — Convidar Participantes para a lista")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN009 — Convidar Participantes para a lista]</h6>

## c) Troca de informações sobre as preferências de presentes
Os participantes poderão informar que presente gostaria de receber, bem como as características do mesmo. Estas informações podem ser, por exemplo, a loja onde o presente pode ser comprado; um link para compra online do produto; detalhes de tamanho e cor; e o que mais for necessário para facilitar a identificação do presente desejado. Para cadastrar sua sugestão de presente, basta o usuário selecionar a lista desejada clicando no ícone do "olhinho" e depois clicar na aba com um ícone de "dólar" e em seguida clicar no ícone "+".

![Preview](images/functionality/FUN014B.png?raw=true "Figura FUN014B — Seleção da lista desejada")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN014B — Seleção da lista desejada]</h6>

Feito isso, será exibida uma Popup com um input onde o usuário deverá colocar um título para a sua sugestão e um outro input para ele descrever resumidamente as características do presente que gostaria de receber, conforme Figura FUN015.

![Preview](images/functionality/FUN015B.png?raw=true "Figura FUN015B — Cadastro de Usuário")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN015B — Cadastro da Sugestão de Presente]</h6>

## d) Realização do sorteio sem que haja confusão - sortear a si próprio
O sorteio só poderá ser realizado pelo administrador da lista e há garantia de que não haverá sorteios inválidos, ou seja, um participante presenteando a si próprio ou um participante sendo presenteado por mais de um participante da lista. Assim que o sorteio for realizado os participantes receberão uma notificação informando-os sobre o sorteio.
O sorteio será justo e sem trapaças, não sendo possível selecionar critérios para favorecer ou desfavorecer o sorteio. Sendo assim, o sorteio será completamente aleatório.
Para realizar o sorteio é muito simples: basta o administrador da lista clicar no terceiro na da lista desejada na tela principal do MAS. Em seguida, ele será questionado se deseja realmente realizar o sorteio. Caso responda sim, o sorteio será realizado, conforme ilustra a Figura FUN017.

![Preview](images/functionality/FUN017B.png?raw=true "Figura FUN017B — Realização do Sorteio da Lista")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN017B — Realização do Sorteio da Lista]</h6>

## e) Interface de cadastro de usuário
Para acessar a aplicação, todos os usuários deverão efetuar o cadastro prévio para ter acesso aos dados da lista ou para criar novas listas de amigo secreto.
Para realizar o cadastro é necessário que o usuário informe seu número de telefone com DDD, seu nome ou apelido e defina uma senha de acesso. Assim que o usuário inserir o código corretamente, ele será redirecionado para a tela principal da aplicação.
Estes dados podem ser alterados através da tela de Perfil do Usuário, caso ele necessite.

![Preview](images/functionality/FUN002.png?raw=true "Figura FUN002 — Cadastro de Usuário")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN002 — Cadastro de usuário]</h6>

## f) Interface para realizar login
Na tela de login o usuário deverá informar o número de telefone com DDD e a senha que foram cadastrados previamente. Se os dados estiverem corretos ele será redirecionado para a tela principal da aplicação. É nesta tela que eles poderão realizar o cadastro, clicando em "cadastre-se!". Também é possível redefinir a senha clicando em "Esqueceu sua senha?".

![Preview](images/functionality/FUN003.png?raw=true "Figura FUN003 — Tela de Login")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN003 — Tela de Login]</h6>

Ao clicar em "Esqueceu sua senha?" será exibida uma Popup solicitando ao usuário que informe o telefone cadastrado com DDD.

![Preview](images/functionality/FUN004.png?raw=true "Figura FUN004 — Recuperação de Senha")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN004 — Recuperação de Senha]</h6>

## g) Interface para visualizar e editar o perfil
Clicando na aba "Perfil" o usuário poderá editar seus dados cadastrais, caso necessite. Será possível alterar dados como nome e avatar. Não será possível alterar o número de telefone que foi cadastrado pelo usuário.

![Preview](images/functionality/FUN020.png?raw=true "Figura FUN020 — Visualização e edição de Perfil - Nome")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN020 — Visualização e edição de Perfil - Nome]</h6>

A imagem do avatar é definida inicialmente com uma imagem default do sistema. O usuário poderá alterar seu avatar uma única vez e a escolha da imagem é realizada de forma randômica pela aplicação, ou seja, existe uma biblioteca de avatares no App MAS. Quando o usuário escolhe alterar seu avatar o sistema automaticamente escolhe uma dessas imagens da biblioteca. Assim que essa imagem for aleatoriamente escolhida ela é salva automaticamente e o usuário não pode mais alterá-la. Alguns usuários poderão ficar um avatar engraçado, o que deixa a brincadeira através do App mais divertida.

![Preview](images/functionality/FUN020B.png?raw=true "Figura FUN020B — Visualização e edição de Perfil - Avatar")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN020B — Visualização e edição de Perfil - Avatar]</h6>


## h) Visualização do respectivo amigo secreto, obtido após a realização do sorteio
Cada participante poderá visualizar o seu amigo secreto correspondente, à quem deverá presentear. Para saber qual o seu amigo secreto que foi sorteado o usuário deverá selecionar a lista desejada e depois clicar na quarta aba, a aba que possui um "emoticon sorrindo". Por segurança, o amigo secreto não será exibido imediatamente ao acessar esta aba. Para ver quem é o amigo secreto, o usuário deverá "revelar" seu amigo secreto clicando no ícone do cadeado, conforme Figura FUN021.  

![Preview](images/functionality/FUN021.png?raw=true "Figura FUN021 — Visualização do amigo secreto Sorteado - Escondido")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN021 — Visualização do amigo secreto Sorteado - Escondido]</h6>

Assim que o usuário clica no cadeado, o sistema mostra quem é seu amigo secreto, ou seja, a quem deve presentear.

![Preview](images/functionality/FUN021B.png?raw=true "Figura FUN021B — Visualização do amigo secreto Sorteado")
<h6>Fonte: Desenvolvido pelo autor do Projeto [Figura FUN021B — Visualização do amigo secreto Sorteado]</h6>

O administrador da lista não terá, em hipótese alguma, a opção de visualizar o resultado geral do sorteio. Ele somente poderá ver quem é seu próprio amigo secreto - no caso em que esteja participando da brincadeira.
