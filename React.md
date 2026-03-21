# React

## Configurar VSCODE
### ESLint
Instale a extensão EsLint do VS Code e no arquivo eslint.config.js digite:

	    rules: {
 	     '...,
 	     'react/prop-types': 'off',
 	   },


### Prettier
	npm install --save-dev prettier

no arquivo eslint.config.js:

	...
	import prettier from  'eslint-config-prettier';
	export default [
	...,
	prettier
	];
instale a extensão do Prettier para VS Code depois disso.

Em extensions, procure por Format on save e marque a caixa de diálogo 

## Iniciar projeto com vite
Antes de iniciar o projeto, é necessário instalar no NodeJS.

	npm create vite@latest
	npm install
	npm run dev

