# 🐧 Agente CS2 para Linux
Este é um agente Flask para Linux que estou desenvolvendo e testando para gerenciar servidores do Counter-Strike 2 (CS2). Já criei anteriormente um agente para Windows e um painel de controle para Windows, e agora estou expandindo a solução para ambientes Linux.
Este agente permite iniciar, parar e monitorar servidores CS2 de forma remota via API HTTP.

V Verso windows 11 e 10 https://github.com/Annabel369/PanelCS2_PHP_RCON2

# 🚀 Como executar
1. 	Clone o repositório:

git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio

2. 	Crie e ative o ambiente virtual:

   	    python3 -m venv venv
        source venv/bin/activate

4. 	Instale as dependências:

5. 	    pip install -r requirements.txt

6. 	Configure a porta no :

          config.py
          AGENT_PORT = 27018  # ou a porta desejada

8. 	Inicie o agente:

              python3 app.py


O agente estará disponível em .

# 📡 Endpoints disponíveis
- POST /start_server – Inicia o servidor CS2
- POST /stop_server – Encerra o servidor CS2
- GET /status – Retorna o status atual do servido


      curl -X POST http://localhost:27033/start_server

      curl -X POST http://localhost:27033/stop_server

      curl http://localhost:27033/status
