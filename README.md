# TCC
Para conseguirmos executar o projeto é necessário realizar o download de dependências e executar operações:
	Node.js: apenas as versões LTS são suportadas (v14 e v16). 
	Yarn
	PostgreSQL 14.0

Pré-requisito: criar um banco de dados denominado "api_hospital" dentro do PostgresSQL para conseguir realizar a execução do projeto. 
Execução dos Projetos: para cada projeto é necessário acessar o diretório do mesmo em um terminal diferente.
API_Hospital: Inicialmente instalar as dependências com o seguinte comando
yarn install
Logo após, executar o seguinte comando para iniciar a aplicação:
yarn develop
Reconhecimento_ facial: Começando Buildar a imagem do Docker. 
Comece criando a imagem docker com um nome definido. 
  Obs: essa ação pode demorar um certo tempo. 
   docker build -t face_servico .
Rodar a imagem do Docker 
Inicie a imagem e encaminhe a porta 8080. 
Opcionalmente, vincule um diretório local a /root/faces para fornecer um local para imagens predefinidas que serão registradas na hora de início
   docker run -d -p8080:8080 -v faces:/root/faces face_servico
Totem_atendimeto: Instale as dependências com o seguinte comando
  yarn install
Logo após, executar o seguinte comando para iniciar a aplicação:
  yarn run dev
