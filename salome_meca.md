# Salome Meca

## instalar o singulary

Acessar e baixar o arquivo .deb:

	https://github.com/sylabs/singularity/releases

Instalar o singularity:

	sudo dpkg -i singularity-container_*.deb

	sudo apt-get install -f  

Verificar a instalação:

	singularity --version

	ls -l /usr/libexec/singularity/bin/starter-suid

# Instalar e executar o salome meca

	singularity run --app install salome_meca-lgpl-2024.1.0-1-20240327-scibian-11.sif


Para executar o Salome Meca, colar no terminal o comando (no diretório de instalação):

	./salome_meca-lgpl-2024.1.0-1-20240327-scibian-11

	which singularity

	hash -r # Limpa o cache de comandos do shell