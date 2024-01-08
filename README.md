# Gherkin

Este repositório tem como finalizadade exibir um exemplo de escrita de uma user story em Gherkin
<br>
Feature: Login na Udemy<br>
<br>
  Eu como usuário da udemy<br>
  Quero ter acesso a plataforma<br>
  Porque assim consigo fazer meus cursos para me qualificar<br>
<br>
Background: Acesso a plataforma<br>
Given que sou usuário da Udemy <br>
When quando adiciono meus dados de acesso<br>
<br>
Scenario: Login com dados corretos por email e senha<br>
E tanto o email como a senha estão corretos para o login<br>
Then consigo realizar meu login no sistema da Udemy<br>
<br>
Scenario Outline: Login com dados corretos por redes<br>
E insiro os dados de acesso do <rede> de uma conta válida<br>
Then consigo realizar meu login no sistema da Udemy<br>
<br>
Examples: <br>
	|rede    |<br>
	|Google  |<br>
	|Facebook|<br>
	|Apple   |<br>
<br>
Scenario: Login com dados incorretos<br>
E eles estão incorretos para login<br>
Then não consigo realizar meu login na Udemy<br>
But aparece uma mensagem informando quais dados estão incorretos para acesso
