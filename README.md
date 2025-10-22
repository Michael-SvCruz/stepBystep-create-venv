# Criando um ambiente virtual 
## Objetivo
Esse repositório tem o objetivo de mostrar o passo a passo de forma simples e direta a como criar um ambiente virtual (venv) localmente para trabalhar de forma segura em seus projetos.

**O processo é executado no prompt wsl-ubuntu do windows 11**

## Passos:
1. Navegue até a pasta que deseja criar a venv; <br/><br/>
2. Criar o diretório (pasta) para o ambiente (nome que desejar)
	```bash
	mkdir <nome_escolhido>
	```
 3. Acessar a pasta
	```bash
	cd <nome_escolhido>
	```
 4. Criar o ambiente venv (por padrão o ambiente é criado com o nome "venv")
	```bash
	python3 -m venv venv	
	```
5. Ativar o ambiente venv (obs. deve estar dentro da pasta criada)
	```bash
	source venv/bin/activate
   ```
 **Após ativar o ambiente virtual (venv) é dessa forma que deve aparecer<br/>**
