# Consolidação dos dados
Abaixo a descrição e imagens da validação do app MAS - Meu Amigo Secreto.

## Primeira etapa da Validação
Na primeira etapa foi desenvolvido um protótipo. Foram coletadas e analisadas as informações fornecidas pela própria loja de aplicativos do Google, dados sobre o aplicativo publicado e que são destinados aos desenvolvedores.

Na Figura VAL000 é possível observar as 3 versões do app MAS que foram geradas.
![Preview](images/validation/VAL000.png?raw=true "Figura VAL000 - App MAS publicado na loja do Google")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL000 - App MAS publicado na loja do Google]</h5>

A versão piloto foi publicada no dia 10/08/2018. Através dela foi obtido o feedback sobre a concepção da ideia. Também houve feedback de usuários que auxiliaram no desenvolvimento de melhorias e correções, tanto do aplicativo quanto da ideia conceitual do projeto.

![Preview](images/validation/VAL001.png?raw=true "Figura VAL001 - Relatório do app MAS na loja do Google")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL001 - Relatório do app MAS na loja do Google]</h5>

Na Figura VAL001 podemos observar que houve um grande número de downloads do aplicativo e também um alto valor de desinstalações. Deste total de instalações, apenas dois usuários deram feedback. Um destes usuários relatou uma falha em que estava sendo possível visualizar a lista de amigo secreto de qualquer usuário, ou seja, que todas as listas estavam visíveis a qualquer usuário do MAS - quando na verdade, apenas quem criou e quem participa da lista poderiam visualizá-las.

![Preview](images/validation/VAL002.png?raw=true "Figura VAL002 - Avaliação de usuário na loja do Google")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL002 - Avaliação de usuário na loja do Google]</h5>

Imediatamente a aplicação foi bloqueada e foi repensada a estrutura do banco de dados, de forma que estes dados ficassem mais seguros. Com base nisso, foi adotada a estrutura atual do banco de dados, que pode ser visto no <a href="https://github.com/djeico/TCC-Meu-Amigo-Secreto/blob/master/estrutura-banco-dados.md#representa%C3%A7%C3%A3o-do-banco-de-dados---collections">Github</a> <https://github.com/djeico/TCC-Meu-Amigo-Secreto/blob/master/estrutura-banco-dados.md#representa%C3%A7%C3%A3o-do-banco-de-dados---collections>.
A nova estrutura encapsula todos os dados da lista, de forma que falhas nesse tipo de segurança acabam se tornando menos provável.

A estrutura anterior era mantida no Realtime Database, também do Firebase, conforme pode ser observado na Figura COL007.

![Preview](images/collection/COL007.png?raw=true "Figura COL007 - Antiga estrutura do banco de dados")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura COL007 - Antiga estrutura do banco de dados]</h5>

## Segunda etapa da Validação
Na segunda etapa, após análise dos dados coletados na primeira etapa, o aplicativo foi corrigido e melhorado conforme as necessidades e problemas identificados na primeira etapa da validação. Depois foi gerada uma nova versão (Beta fechada) e disponibilizada apenas para uso real na empresa Salbego Laboratório Farmacêutico Ltda. A ideia foi validar as alterações relacionadas à segurança e correções de interface que foram realizadas no aplicativo. Ao todo foram 18 usuários que participaram da lista de amigo secreto e realizaram o teste.

![Preview](images/validation/VAL003.png?raw=true "Figura VAL003 - Relatório do app MAS para a segunda versão")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL003 - Relatório do app MAS para a segunda versão]</h5>

Como haviam 4 usuários com smartphone da Apple, foi desenvolvida uma interface web que possibilitasse ao usuário acessar a lista de amigo secreto, cadastrar e visualizar preferências de presentes e visualizar o seu amigo secreto que foi sorteado.
A brincadeira feita através do MAS ocorreu como o esperado e ao final todos revelaram seus respectivos amigos secretos.
O arquivo "*.json" com o banco de dados utilizado nesta etapa da validação está disponível no <a href="https://github.com/djeico/TCC-Meu-Amigo-Secreto/blob/master/database/DB_FASE2.json">Github<a>, no link <https://github.com/djeico/TCC-Meu-Amigo-Secreto/blob/master/database/DB_FASE2.json>

## Terceira etapa da Validação
Na terceira etapa da Validação o App MAS foi utilizado por um grupo de 17 pessoas.

![Preview](images/validation/VAL014.png?raw=true "Figura VAL014 - Relatório do app MAS para a segunda versão")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL014 - Relatório do app MAS para a terceira versão]</h5>

Alguns usuários optaram por utilizar a versão PWA do MAS, sendo que no total de 8 decidiram utilizar o app Nativo para Android, conforme Figura VAL015.

![Preview](images/validation/VAL015.png?raw=true "Figura VAL015 - Relatório do app MAS para a segunda versão")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL015 - Relatório do app MAS para a terceira versão]</h5>





### Perfil dos Usuários
Conforme demonstrado na Figura VAL005, verificou-se que a maioria dos usuários do app MAS possui mais de 40 anos de idade. Sendo assim, é um grande desafio introduzir uma solução digital para uma brincadeira que faz parte da vida de muitas pessoas. É importante salientar que houve um pequeno equívoco na definição dos critérios da faixa etária desta questão: onde consta a alternativa "12 - 12 anos", deve-se entender 12 - 18 anos. Este equívoco não influenciou no resultado deste teste.

![Preview](images/validation/VAL005.png?raw=true "Figura VAL005 - Pergunta sobre perfil do usuário.")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL005 - Pergunta sobre perfil do usuário.]</h5>

Na Figura VAL006 é possível observar que a utilização de smartphones por parte dos usuários é relativamente alta, sendo assim, subentende-se que os usuários estão bastante familiarizados com o acesso a aplicativos móveis.

![Preview](images/validation/VAL006.png?raw=true "Figura VAL006 - Pergunta sobre perfil do usuário.")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL006 - Pergunta sobre perfil do usuário.]</h5>

Nota-se que 41,2% dos usuários que responderam à avaliação já participaram do processo de criação do amigo secreto, conforme ilustrado na Figura VAL007. Estes usuários, melhor do que os demais, poderão avaliar todas as funcionalidades do app MAS, bem como sua eficiência e eficácia num contexto geral.

![Preview](images/validation/VAL007.png?raw=true "Figura VAL007 - Pergunta sobre perfil do usuário.")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL007 - Pergunta sobre perfil do usuário.]</h5>

Na Figura VAL008 é possível observar que mais de 90% dos usuários que participaram da avaliação já participaram da brincadeira do amigo secreto. Estes dados ajudam a validar a usabilidade, eficiência e eficácia do app MAS, pois subentende-se que pelo fato de os usuários já estarem familiarizados com a brincadeira, poderão avaliar de forma mais realista as funcionalidades disponíveis no app MAS.

![Preview](images/validation/VAL008.png?raw=true "Figura VAL008 - Pergunta sobre perfil do usuário.")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL008 - Pergunta sobre perfil do usuário.]</h5>

Na Figura VAL009 podemos ver quantos dos usuários do MAS que responderam ao questionário já utilizou alguma ferramenta informatizada para realizar o amigo secreto. Existem duas necessidades: a primeira é atender às expectativas dos 23% dos usuários que já utilizaram alguma outra solução informatizada, pois inevitavelmente haverão comparações. A segunda é fisgar os usuários que estão conhecendo agora uma maneira, de certa forma, inovadora de realizar a brincadeira do amigo secreto.

![Preview](images/validation/VAL009.png?raw=true "Figura VAL009 - Pergunta sobre perfil do usuário.")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL009 - Pergunta sobre perfil do usuário.]</h5>


### Funcionalidade
Na Figura VAL010 constatou-se que todos os usuários do app MAS que responderam ao questionário entenderam que cadastrar e visualizar a preferência de presentes, realizar o sorteio do amigo secreto sem subterfúgios do administrador e sigilo na visualização do amigo secreto sorteado ajudaram na realização do amigo secreto através do smartphone.

![Preview](images/validation/VAL010.png?raw=true "Figura VAL010 - Pergunta sobre perfil do funcionalidades do app MAS.")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL010 - Pergunta sobre perfil do funcionalidades do app MAS.]</h5>

### Eficácia
Na Figura VAL011 foi verificada a eficácia na utilização do MAS para a realização do amigo secreto pelo smartphone. Todos os usuários que responderam ao questionário informaram que ele cumpriu o propósito, conforme era esperado para a solução.

![Preview](images/validation/VAL011.png?raw=true "Figura VAL011 - Pergunta a eficácia do app MAS.")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL011 - Pergunta a eficácia do app MAS.]</h5>

### Eficiência
Na Figura VAL012 foi verificada a eficiência do MAS na realização da brincadeira, principalmente em relação ao sorteio. Com base no resultado, pode-se concluir que o sorteio foi realizado corretamente e conforme o proposto pela solução.

![Preview](images/validation/VAL012.png?raw=true "Figura VAL012 - Pergunta a eficiência do app MAS.")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL012 - Pergunta a eficiência do app MAS.]</h5>

### Usabilidade
A Figura VAL013 ilustra a opinião dos usuários do MAS que responderam ao questionário, sobre a utilização da brincadeira no app.
As respostas obtidas nesta questão foram bastante satisfatórias, pois demonstram que a solução proposta foi de fácil utilização pela maioria dos usuários. O objetivo era trazer uma solução de fácil utilização, que permitisse a realização do sorteio do amigo secreto de forma segura e que não permitisse ao administrador da lista burlar o sorteio.

![Preview](images/validation/VAL013.png?raw=true "Figura VAL013 - Pergunta sobre usabilidade do app MAS.")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL013 - Pergunta sobre usabilidade do app MAS.]</h5>
