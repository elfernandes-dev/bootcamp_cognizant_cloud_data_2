#Introdução ao Git e ao GitHub
##Introdução
 - Git = Criado por _Linus Torvalds_
 - GitHub = Mantido pela _Microsoft_
	
##Conceitos
 - SHA1 (Secure Hash Algorithm = Algoritmo de Hash Seguro) projetado pala NAS (Agência de Segurança Nacional dos EUA)
 	_Cria um conjunto de caracteres de 40 dígitos_
 - Objetos (Blobs; Trees; Commits)
	_Blobs_ -> Contém os metadatas do arquivo dentro do git.
	_Trees_ -> Armazenam Blobs.			
	_Commits_ -> ‘Junta tudo’. Aponta para a Tree, Parente (último Commits realisado), Autor, Mensagem e Timestamp (Carimbo de tempo)
				

##SSH e Token
###Chave SSH
 - ssh-keygen -t ed25519 -C meuemail@email.com _-> Criar SSH_
 - ssh$ cat id_ed25519.pub _-> Icluir essa SSH no GitHub_
 - eval $(ssh-agent -s) _-> Acionar o agente para validação_
 - ssh$ ssh-add id_ed25519 _- > Ativar as configuração_

###Token (Segunda opção de validação, mas ela solicita um ‘prazo de validade’0
 - Developer settings > Personal access tokens > Generate new token
	Incluir:
		Note (tag)
		Tempo para expiração
		Scope (repo atende o padrão)
		Após gerar o token salve num lugar seguro e uso quando o git solicitar
		

###Uso do Markdown
[Link sobre o Markdown] (https://www.markdownguide.org/basic-syntax)
