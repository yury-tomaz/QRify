# QRify API 🚧 (em fase de desenvolvimento)

Este projeto tem como objetivo criar uma API para geração de códigos QR, onde o usuário pode gerar um QR code e alterar a URL associada a ele a qualquer momento, mantendo a imagem QR code impressa constante.

## Tecnologias Utilizadas

- Node.js
- Biblioteca [qrcode](https://www.npmjs.com/package/qrcode) ou [qrcode-generator](https://www.npmjs.com/package/qrcode-generator)
- Express (para as rotas)

## Instalação

Para instalar as dependências do projeto, execute o seguinte comando no terminal:

npm install

## Rotas

A API oferece as seguintes rotas:

### GET /qr-code

Esta rota retorna a página de geração de QR code.

Exemplo de requisição:

GET http://localhost:3000/qr-code


### POST /qr-code

Esta rota gera o QR code a partir da URL fornecida no corpo da requisição.

Exemplo de requisição:

POST http://localhost:3000/qr-code

{
"url": "https://www.example.com"
}


Exemplo de resposta:

{
"qrCode": "data:image/png;base64,..."
}


## Uso

1. Inicie o servidor executando o seguinte comando no terminal:

npm start


2. Acesse a URL `http://localhost:3000/qr-code` em seu navegador para ver a página de geração de QR code.

3. Insira a URL desejada e clique no botão "Gerar QR Code".

4. A imagem do QR code gerado pode ser salva e impressa.

## Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

