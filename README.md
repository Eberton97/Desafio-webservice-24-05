Desafio webservice 24/05
# Desafio Webservices - Imersão 360

Este repositório contém a resolução das 6 etapas propostas no desafio de Webservices utilizando a API pública [DummyJSON](https://dummyjson.com/docs).

## Etapas realizadas:

### 1. Listar todos os usuários
**Método:** GET  
**Endpoint:** `https://dummyjson.com/users`  
![1 - Lista de usuários](https://github.com/user-attachments/assets/d4cd5510-7eab-4c35-9cb7-9eb22e029c51)

Depois **Send**

### 2. Buscar informações de um usuário específico

**Método:** GET

**Endpoint:** `https://dummyjson.com/users/1`  
![2 - Buscar usuário](![Image](https://github.com/user-attachments/assets/ffbba638-9ed6-48bb-9471-a40626050915)

Depois **Send**

### 3. Criar um novo usuário
**Método:** POST 
Aba: Body ( corpo )
**Comando:** 
{
  "firstName": "Bruno",
  "lastName": "Santos",
  "maidenName": " Eberton",
  "age": 28,
  "gender": "male",
  "email": "eberton.bruno07@aluno.ifce.edu.br",
  "phone": "+55 88 993540627",
  "username": "eberton07",
  "password": "Prodigio97$",
  "birthDate": "1997-02-02",
  "image": "https://randomuser.me/api/portraits/men/75.jpg",
  "bloodGroup": "O+",
  "height": 167,
  "weight": 72.6,
  "eyeColor": "brown",
  "hair": {
    "color": "black",
    "type": "curly"
  },
  "domain": "eberton.dev",
  "ip": "192.168.1.100",
  "address": {
    "address": "Rua Gabriel Arcanjo, 67",
    "city": "Bela Cruz",
    "coordinates": {
      "lat":  -3.054,
      "lng": -40.1741
    },
    "postalCode": "62570000",
    "state": "CE"
  },
  "macAddress": "00:1B:44:11:3A:B7",
  "university": "IFCE/Sobral",
  "bank": {
    "cardExpire": "12/28",
    "cardNumber": "1234-5678-9876-5432",
    "cardType": "visa",
    "currency": "BRL",
    "iban": "BR2900000000000000000000000"
  },
  "company": {
    "address": {
      "address": "Rua. Gabriel Arcanjo, 67",
      "city": "Bela Cruz",
      "coordinates": {
        "lat":  -3.054,
        "lng": -40.1741
      },
      "postalCode": "62570000",
      "state": "CE"
    },
    "department": "TI",
    "name": "Eberton Tech",
    "title": "Desenvolvedor"
  },
  "ein": "12-3456789",
  "ssn": "123-45-6789",
  "userAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64)"
}
**Endpoint:** `https://dummyjson.com/users/add`  
![3 - Criar usuário](![Image](https://github.com/user-attachments/assets/cca0e3aa-eaa5-4252-b911-8dd5367e763e)

Depois **Send**

### 4. Atualizar a senha
**Método:** PUT 
**Aba:** Body
comando: 
{
"password":"Nuvem2025!" 
}

**Endpoint:** `https://dummyjson.com/users/1`  
![4 - Atualizar senha](![Image](https://github.com/user-attachments/assets/a19e88b5-6b2f-4f38-b81c-2479de7616af)

Depois **Send**

### 5. Fazer login com Michael Michaels (ou outro usuário funcional)
**Método:** POST 
**Aba:** Body
Comando
{
  "username": "michaelw",
  "password": "michaelwpass"
}
**O usuário " Michael Michaels " não consta na lista de usuários, então, usei o segundo ID.**

**Endpoint:** `https://dummyjson.com/auth/login`  
![5 - Login](![Image](https://github.com/user-attachments/assets/cf50134a-46b8-4dcc-abb7-798a473b5910)

Depois **Send**

### 6. Verificar se Estar logado

**Método:** GET  
**Aba:** Headers

     Preencha assim:

Name:

Authorization

Value: token do usuário 

Bearer ( tem que ter no início e seguido de um espaço antes do token )

**Endpoint:** `https://dummyjson.com/auth/me`  
**Header:** Authorization: Bearer `SEU_TOKEN`  
![6 - Dados logado]
![Image](https://github.com/user-attachments/assets/31b05076-e769-4744-8c6e-5342536d0875)

ou 

simpficando

![Image](https://github.com/user-attachments/assets/f50bfde2-3b44-41fa-adc6-9c7c141da4b3)

Depois **Send**
