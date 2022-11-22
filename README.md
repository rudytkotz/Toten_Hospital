# TCC

Para conseguirmos executar o projeto é necessário realizar o download de algumas dependencias e realizar algumas operações:

Node.js: apenas as versões LTS são suportadas (v14 e v16).
yarn para executar os scripts de instalação da CL
PostgreSQL 14.0


Pré-requisito:
Criar um banco de dados denominado "api_hospital" dentro do PostgresSQL para conseguir realizar a execução do projeto




Execução dos Projetos:
Para cada projeto é necessario acessar o diretorio do mesmo em um terminal diferente.


API_Hospital

Inicalmente instalar as dependencias com o seguinte comando

yarn install

Então somente executar o seguinte comando e iniciara a aplicação

yarn develop




Reconhecimento facial

Começando
Buildar a imagem do Docker
Comece criando a imagem docker com um nome definido. Isso pode demorar um pouco.

docker build -t face_servico .


Rodar a imagem do Docker
Inicie a imagem e encaminhe a porta 8080. Opcionalmente, vincule um diretório local a /root/faces para fornecer um local para imagens predefinidas que serão registradas na hora de início

docker run -d -p8080:8080 -v faces:/root/faces face_servico




Totem atendimenro

Inicalmente instalar as dependencias com o seguinte comando

yarn install

Então somente executar o seguinte comando e iniciara a aplicação

yarn run dev
