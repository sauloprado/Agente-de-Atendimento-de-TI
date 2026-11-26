# Agente de Atendimento de TI

![Capa do projeto](capa-repositorio.png)

Projeto educacional da DIO. A Aurora Digital é fictícia.

O chat foi feito em Python com Flask e HTML. As respostas automáticas são locais, selecionadas por palavras-chave configuradas em respostas.json. Não usa IA, não envia mensagens a serviços externos e não acessa sistemas corporativos.

## Baixar

[Baixar o projeto completo em ZIP](https://github.com/sauloprado/Agente-de-Atendimento-de-TI/raw/refs/heads/main/Agente-de-Atendimento-de-TI.zip)

O pacote inclui o aplicativo, as respostas, o prompt, a interface, a imagem e os testes.

## Executar no Windows

Requer Python 3.10 ou superior. No PowerShell, na pasta do projeto:

~~~powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
python app.py
~~~

Abra http://127.0.0.1:5000. Não é necessária chave de API.

Edite respostas.json para ajustar palavras-chave e respostas. Perguntas que não correspondam às regras recebem uma orientação padrão. O aplicativo não consulta status, estoque, licenças ou solicitações, nem abre ou encaminha chamados.

## Testes

~~~powershell
python -m unittest discover -s tests
~~~

## Arquivos principais

- app.py: servidor web Flask e validação das mensagens.
- responder.py e respostas.json: classificação local e base de respostas.
- templates e static: interface HTML, CSS e JavaScript.
- prompt.md: instruções originais do agente.

## Autor

Saulo Prado
