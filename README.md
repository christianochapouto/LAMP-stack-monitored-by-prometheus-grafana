Primeiro clone o repositorio 
git clone https://github.com/christianochapouto/PHP-webserver-with-monitoring/

Mova para o diretorio resultante
cd PHP-webserver-with-monitoring

Suba do stack do serviço do webserver PHP
Docker stack deploy -c docker-compose.yml [nome do stack]

vá para a pasta do serviço de monitoramento
cd monitoring

Realize o mesmo comando, com o nome desejado para o stack
Docker stack deploy -c docker-compose.yml [nome do stack]

Você pode acessar o webserver via "0.0.0.0".
Você pode acessar os graficos do grafana via 0.0.0.0:8080.
Você pode acessar o "expression browser" do prometheus via 0.0.0.0:9090

Você pode editar/criar arquivos na pasta www que serão as paginas do webserver.
