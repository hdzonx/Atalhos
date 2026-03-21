# Ambiente virtual no python

	python3 -m venv .venv

	source .venv/bin/activate

Criar arquivo Requirements.txt

	pip freeze > requirements.txt


# Sequência de comandos para criar lib rust para python


	# (replace string_sum with the desired package name)
	mkdir string_sum
	cd string_sum
	python -m venv .env
	source .env/bin/activate
	pip install maturin

	maturin init
	maturin develop

Depois disso pode-se criar um arquivo python (ex. main.py) na raiz do projeto e importar a biblioteca:

	import string_sum

	print(string_sum.sum_as_string(2,4))

## Importante

Uma vez feitas alterações na biblioteca, é necessário recompilar:

	cargo clean
	maturin develop





