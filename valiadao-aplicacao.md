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


![Preview](images/validation/VAL005.png?raw=true "Figura VAL005 - Pergunta número um.")
<h5>Fonte: Desenvolvido pelo autor do Projeto [Figura VAL005 - Pergunta número um.]</h5>
