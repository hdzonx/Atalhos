# Instalação e configuração no linux
Acessar a página da linguagem Go e baixar o arquivo tar.gz

abrir o terminal na pasta em que o arquivo de instalação do Go se encontra. 

Verificar se a hash do arquivo baixado confere com a do site:

	sha256sum go1.X.X.linux.amd64.tar.gz

Caso exista uma versão anterior do Go, é necessário removê-lo:

	rm -rf /usr/local/go

Em seguida extrair e instalar o arquivo conforme o exemplo:

	sudo tar -C /usr/local -xzf go1.X.X.linux.amd64.tar.gz

Abrir o arquivo de configuração:

	nano ~/.bashrc

No arvquivo de configuração, desça até o final e inclua:

	export PATH=$PATH:/usr/local/go/bin
	export GOPATH=$HOME/go
	export PATH=$PATH:$GOPATH/bin

Para salvar o arquivo:

	ctrl+o
	Enter
	crtl+x

Em seguinda, o arquivo pode ser carregado:

	source ~/.bashrc

Se tudo tiver dado certo, aparecerá a versão do Go em:

	go version












