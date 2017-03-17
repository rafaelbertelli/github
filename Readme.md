Bem vindo!
==========
Este é um repositório teste para verificar como o  Git funciona.
==================================================================

[Git]
	Estes são comandos de Git, utilizados no Git.CMD

		*
		git init
		Inicializa um diretório Git na pasta
		
		*
		git status
		Verifica o status do Branch
		
		*
		git add Arquivo.js
		Adiciona o arquivo ao Branch, mas sem commit
		
		*
		git commit -m "Mensagem de alteração do arquivo"
		Commit do arquivo e passa mensagem de log
		
		*
		git commit -am "mensagem"
		Adiciona todos os arquivos alterados e comenta
		
		*
		git log
		Me mostra os logs de alteração dos arquivos		
		
		*
		git log --decorate
		Mostra o log com informação de troca de branch, etc
		
		*
		git log --author="Rafael"
		Mostra logs de author específico
		
		*
		git shortlog
		Mostra logs dos authors e suas alterações
		
		*
		git shortlog -sn
		Mostra somatória de alterações dos authors
		
		*
		git log --graph
		Mostra o repositório de forma grafica
		
		*
		git show 7f39ed4536436bb3d804de19d8b947c262c8ddcc
		Passar a hash para ver exatamento a alteração feita no arqivo
		
		*
		git diff
		Mostra a diferença do arquivo que estou mexendo antes de eu fazer commit
		
		*
		git diff --name-only
		Diz somente o nome do arquivo modificado
		
		*
		git checkout Nomedoarquivo.extencao
		Carrega um arquivo do git pra sua maquina, pode sobrepor um arquivo
		
		*
		git reset HEAD
		Remove do staged, que é quando eu faço git add no arquivo
		
		*
		git reset --soft [passo a hash do arquivo anterior ao q eu quero deletar]
		Deleta do último commited até a hash que vc passar mas o arquivo fica em staged preparado para o commit de novo
		
		*
		git reset --mixed [passo a hash do arquivo anterior ao q eu quero deletar]
		Deleta do último commited até a hash que vc passar mas o arquivo fica fica preparado para ir para o staged. Com isso, posso chamar o checkout para sobrepor minha alteração
		
		*
		git reset --hard [passo a hash do arquivo anterior ao q eu quero deletar]
		Mata o commit e qualque modificação
		
		
[GitHub]
	Estes são comandos de Git, utilizados no Git.CMD
	
		*
		Criar Repositório -> No próprio GitHub
		
		*
		O próprio GitHub te passa os comando para o CLI
		O nome 'origin' é um nome do repositório original que poderia ser substituido por qq nome.
		
		*
		git remote
		Mostra os repositórios disponíveis
		
		*
		git remote -v
		Mostra as opções do repositório
		
		*
		git push -u origin master
		Envia todos meus arquivos, as moficações para o repositório. O -u serve para trackear e não ter que digitar isso tudo de novo no próximo push. 
		origin -> pra onde vai. master -> de onde vem. Ou seja, vem do branch MASTER e vai pro ORIGIN.
		
		
		*
		git push origin master
		Envia para o repositório de para o ORIGIN para o MASTER
	
	
	[Branch]
		Branch é um ponteiro móvel que leva a um commit.
		Posso apontar um outro Branch para o mesmo commit, ou ter Branchs em commits diferentes
		
			* Vantagens
				Posso modificar meus arquivos sem alterar meu local principal, meu master
				Por exemplo, posso corrigir um Bug enquanto tem outras pessoas trabalhando no Branch Master
				Ele é facilmente desligável
				Posso ter multiplas pessoas trabalhando
				Evita conflito, pois cada branch não interfere em outro e o commit dele para o master entra somente no ponto de destino na linha do tempo, sem conflito com outros usuário, permite tbm a mescla de arquivos alterados.
				
				
		*
		git checkout -b "nome do branch"
		Cria um novo branch e me posiciona nele.
		
		*
		git branch
		Mostra os branch existentes e mostra o asterisco no branch onde estou no momento
		
		*
		git checkout "nome do branch"
		Mudo de branch
		
		*
		git branch -D "nome do branch"
		Deleta o branch indicado
		
		*
				
	
