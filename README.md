# Padrao para criar nome de imagem docker
namespace -> quem esta criando a imagem ou nome da instituicao
repositorio -> nome do repositorio da aplicacao
tag -> versao da aplicacao
## ex: flpmarcos/conversao-temperatura:v1

# Comando para montar a imagem
docker image build -t flpmarcos/conversao-temperatura:v1 .

# Comando para rodar a imagem
-d para rodar em daemon
-p para expor a porta
docker container run -d -p 8080:8080 flpmarcos/conversao-temperatura:v1


# Subir versao para o dockerhub
docker login

# Subir imagem para o repositorio registry
docker push flpmarcos/conversao-temperatura:v1
