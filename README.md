# API Fake - NaEsquina

Esta é a **API Fake** utilizada pelo projeto [NaEsquina](https://github.com/devtatomachado/NaEsquina), criada com **JSON-Server** para simular um backend durante o desenvolvimento.

---
## 🧐 Sobre a API
Esta API foi criada para fornecer dados simulados, como empreendedores e produtos, permitindo que o front-end consuma informações como se estivesse conectado a um backend real.

---

## 🛠 Tecnologias
- [JSON-Server](https://github.com/typicode/json-server)
- Node.js

---

## 📋 Pré-requisitos
Antes de rodar a API, você precisará ter instalado:
- [Node.js](https://nodejs.org/)
- npm ou yarn

---

## 🚀 Como Rodar

Clone o repositório:
```
git clone https://github.com/devtatomachado/NaEsquina-API.git
```

Acesse a pasta do projeto:
```
cd NaEsquina-API
```

Instale as dependências:
```
npm install
```

Inicie a API:
```
npx json-server --watch db.json --port 3001
```

A API estará disponível em:
```
http://localhost:3000
```

---

## 🔗 Endpoints Disponíveis
- **GET /empreendedores** → Lista todos os empreendedores
- **GET /produtos** → Lista todos os produtos
- **POST /empreendedores** → Adiciona um novo empreendedor
- **POST /produtos** → Adiciona um novo produto

---

## 📂 Estrutura do db.json
Exemplo de estrutura do arquivo:
```

 "usuarios": [
    {
      "id": "a1b2",
      "nome": "João Artesão",
      "endereco": "Rua das Flores, 123",
      "documento": "11122233344",
      "email": "joao.artesao@naesquina.com",
      "senha": "senha123",
      "isStore": true,
      "favoritos": [
        {
          "lojaid": "g7h8"
        }
      ],
      "lojaId": "c3d4"
    }
  ]
  "lojas": [
    {
      "id": "c3d4",
      "nomeLoja": "Arte em Madeira do João",
      "UsuarioId": "a1b2",
      "logo": "https://img.freepik.com/vetores-premium/conceito-realista-de-logotipo-de-negocio-corporativo-de-tipo-diferente_1286368-70511.jpg?semt=ais_hybrid&w=740",
      "bio": "Móveis e objetos de decoração em madeira feitos à mão com paixão e precisão. Cada peça é única e carrega a essência da arte da marcenaria tradicional.",
      "produtos": [
        {
          "id": 1751237561548,
          "nome": "Banco Rústico",
          "imagem": "https://images.tcdn.com.br/img/img_prod/889102/banco_sem_encosto_acabamento_rustico_area_externa_1507_1_59f6544d25e3faac75af8eecaaae4044.jpg",
          "descricao": "Banco de madeira maciça, perfeito para áreas externas e varandas.",
          "valor": "120",
          "disponibilidade": "Em estoque"
        }
      ]
    }
  ]
```

---

## 📜 Licença
Este projeto está sob a licença MIT. Sinta-se livre para utilizá-lo.
