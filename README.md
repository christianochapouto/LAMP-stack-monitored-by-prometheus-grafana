#LAMP stack monitorado por prometheus+grafana


Primeiro clone o repositorio <br />
git clone https://github.com/christianochapouto/LAMP-stack-monitored-by-prometheus-grafana <br />
<br />Mova para o diretorio resultante<br />
cd LAMP-stack-monitored-by-prometheus-grafana<br />
<br />Suba o stack do serviço LAMP<br />
Docker stack deploy -c docker-compose.yml [nome do stack]<br />
<br />vá para a pasta do serviço de monitoramento<br />
cd monitoring<br />
<br />Realize o mesmo comando, com o nome desejado para o stack de monitoramento<br />
Docker stack deploy -c docker-compose.yml [nome do stack]<br />
<br />Você pode acessar o webserver via "0.0.0.0".<br />
Você pode acessar os graficos do grafana via 0.0.0.0:8080.<br />
Você pode acessar o "expression browser" do prometheus via 0.0.0.0:9090<br />
Você pode editar/criar arquivos na pasta www que serão as paginas do webserver.<br />
