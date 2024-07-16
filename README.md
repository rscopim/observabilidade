Desafio de Observabilidade da O2B Academy.

Na solução para o Desafio de Observabilidade da O2B Academ foi implemnetado um ambiente de observabilidade usando Prometheus, Grafana e Alertmanager para monitorar uma a aplicação em Python.

Objetivo era criar um ambiente de observabilidade usando Prometheus e Grafana para monitorar uma aplicação.

Minha Solução:
Instalação do Prometheus, Grafana e Alertmanager:
Criei um arquivo docker-compose.yml para definir os serviços Prometheus, Grafana e Alertmanager.
Criei um diretório e iniciei a aplicação em Python.

Métricas na Aplicação:
Acessei a aplicação em http://localhost:3001 e cliquei em "Gerar Erro" e "Calcular Duração".

Configuração do Prometheus:
No arquivo prometheus.yml no diretório prometheus, crie os caminhos para o Alertmanager, Prometheus, Node-exporte, server e a aplicação Python.

Criei uma integração do webhook com o Discord:
Configurei o Alertmanager para enviar alertas para o Discord.
Adicionei um receiver para o Discord com o webhook URL correspondente.

Iniciando o Ambiente:
No diretório raiz do projeto e executei os comando para iniciar:
Server: ./server
Aplicação Python: python app.py
Subir a aplicação: docker-compose up -d
VErificação dos containers: docker-compose ps

Acessando o Prometheus e Grafana:
Acessei o painel do Prometheus em http://localhost:9090 para verificar se a aplicação estava rodando
Acessei o painel do Grafana em http://localhost:3000 para criar um dashboard do prmetheus.
