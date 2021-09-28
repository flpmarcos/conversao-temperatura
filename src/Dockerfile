FROM node
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 8080
CMD ["node", "server.js"]


# Comando para montar a imagem
# docker image build -t conversao-temperatura .


# Comando para rodar a imagem
# -d para rodar em daemon
# -p para expor a porta
# docker container run -d -p 8080:8080 conversao-temperatura