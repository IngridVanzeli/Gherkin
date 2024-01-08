# Gherkin

Este repositório tem como finalizadade exibir um exemplo de escrita de uma user story em Gherkin

Feature: Login na Udemy

  Eu como usuário da udemy
  Quero ter acesso a plataforma
  Porque assim consigo fazer meus cursos para me qualificar

Background: Acesso a plataforma
Given que sou usuário da Udemy 
When quando adiciono meus dados de acesso

Scenario: Login com dados corretos por email e senha
E tanto o email como a senha estão corretos para o login
Then consigo realizar meu login no sistema da Udemy

Scenario Outline: Login com dados corretos por redes
E insiro os dados de acesso do <rede> de uma conta válida
Then consigo realizar meu login no sistema da Udemy

Examples: 
	|rede    |
	|Google  |
	|Facebook|
	|Apple   |

Scenario: Login com dados incorretos
E eles estão incorretos para login
Then não consigo realizar meu login na Udemy
But aparece uma mensagem informando quais dados estão incorretos para acesso
