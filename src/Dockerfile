# é uma boa prática colocar a tag nessa imagem base também 
FROM node:16.13.2
# cria uma pasta chamada app no container
WORKDIR /app
# copia package.json e package-lock.json
# isso é feito para ter vantagem das camadas, já que só vai copiar o resto do cóidigo caso haja alguma modificação nele
COPY package*.json ./
RUN npm install 
# copia tudo e coloca no app/ 
COPY . .
CMD [ "npm", "start" ]