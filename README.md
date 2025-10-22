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
<img src = image/criando_venv_01.png/>

----
## Alguns comando que podem ser úteis
Instala um pacote específico.
```bash
pip install <nome_do_pacote>
```
Instala todos os pacotes listados no arquivo `requirements.txt`.
```bash
pip install -r requirements.txt
```
Lista todos os pacotes instalados **no ambiente virtual**.
```bash
pip list
```
Cria um arquivo `requirements.txt` listando todos os pacotes e suas versões exatas instaladas no ambiente. Este arquivo é crucial para a portabilidade do projeto.
```bash
pip freeze > requirements.txt
```
Desinstala um pacote.
```bash
Desinstala um pacote.
```
Desativa o ambiente virtual e retorna ao prompt normal do sistema.
```bash
deactivate
```
Para remover completamente um ambiente virtual, basta **desativá-lo** primeiro e, em seguida, excluir a pasta que você criou.
```bash
rm -rf test_venv
```
Significado dos argumentos -r e -f
**-r** **Recursivo**. Permite remover diretórios (pastas) e seu conteúdo.
**-f** **Forçar**. Ignora arquivos protegidos  contra escrita e não solicita confirmações.
