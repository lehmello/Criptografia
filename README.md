# Criptografia
Projeto de criptografia em python feito para um trabalho na faculdade

*CRIPTOGRAFIA:*

-PASSO 1
 	Na primeira parte, utilizando o comando ‘while’, o programa pede uma senha pré-definida pelo programador (senha: “APS”), só desbloqueando o passo seguinte assim que a senha for digitada corretamente.
  
 
-PASSO 2
	Assim que a senha for digitada corretamente, será definido uma série de variáveis, primeiro, a ‘senha’, que servira como receptáculo para a mensagem original na qual deseja 	criptografar. Segundo, a variável ‘psw’, que armazenará a mensagem em forma de lista. Terceiro, ‘crp’, que vira a ser a lista dos caracteres já criptografados. E por último,  ‘show’, que se transformara na criptografia final em formato de string.
	 

-PASSO 3
	Agora, transformaremos a mensagem da variável ‘senha’ em uma lista na variável ‘psw’.
	 
	
-PASSO 4
	Utilizando o efeito ‘.reverse’, fazemos a lista ‘psw’ se inverter, transformando-a numa lista espelho da original. O intuito desse passo é dificultar um pouco mais a quebra da criptografia por outros usuários.
	 

-PASSO 5
	Nesse passo, analisaremos a lista ‘psw’ que contém todos os caracteres da mensagem original, e também analisara qual posição do elemento cada caractere se encontra, caso o elemento for número par, armazenara uma serie e letras e números aleatórios na lista ‘crp’.
	 
Caso o elemento for ímpar, armazenara outra série de números e letras na lista ‘crp’ para o caractere equivalente da lista ‘psw’
Caso for o primeiro elemento da lista, ocorrera o mesmo processo com uma outra lista de caracteres e números aleatórios
(PS: as tabelas completas estarão disponíveis no relatório de linhas do código, pois são textos extensivos e atrapalharia a leitura do passo a passo).

-PASSO 6
	No último passo, nós tiramos os caracteres da lista ‘crp’ e passamos para o string ‘show’, facilitando na visualização e mostrando o resultado final ao usuário.


*DECRIPTOGRAFIA:*
	
-PASSO 1
  Utilizando um outro arquivo de codigo, na decriptografia, também utilizamos um comando ‘while’ para proteger o programa com uma senha (APS).
 

-PASSO 2
  Reaproveitamos alguns nomes das variáveis do primeiro código, e aplicamos seus valores. É o mesmo raciocínio da criptografia, a variável ‘msg’ recebera a mensagem criptografada, logo depois, será passada para a lista ‘psw’ através do próximo passo, depois de decriptografada, passara para a lista ‘crp’, logo após, se transformara na variável de string ‘show’ para a visualização do usuário.
 

-PASSO 3
	Aqui, separaremos a mensagem criptografada em uma lista, cada elemento terá oito caracteres, pois esse é o número de caracteres que cada letra criptografada tem. Para isso, usamos duas variáveis inteiras ‘n=0’ e ‘m=8’, assim que o programa verificar os oito primeiros caracteres e os adicionar à lista ‘psw’, o código adicionara mais 8 dígitos as variáveis ‘n’ e ‘m’, assim testando todo o texto digitado no início.
 


-PASSO 4
	Com todos os caracteres da mensagem criptografada separados em grupos de 8, analisaremos cada elemento e sua posição para começarmos o processo de decriptografia. Aplicaremos o efeito reverso do código de criptografia, porém, manteremos a análise de sua posição de elemento, caso o elemento for par. Estamos adicionando um caractere único a lista ‘crp’, caractere esse que é complementar à primeira lista do primeiro código de criptografia, ou seja, estamos substituindo a criptografia pela mensagem original.

-PASSO 5
	Com a lista completa e com a mensagem original, falta apenas inverte-la para voltar a ordem normal, com isso utilizamos novamente o comando ‘.reverse’. 
	 

-PASSO 6
	E para finalizar, colocaremos os caracteres da lista ‘crp’ em um string para melhor visualização do usuário e mostraremos o resultado final.

(Texto retirado da documentação original do projeto, ambos de minha autoria).
