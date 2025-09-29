README.md
# 🛒 Mini Sistema de Gestão de Produtos

## 📌 Sobre o Projeto
Este projeto é um **mini sistema de gestão de produtos** desenvolvido como atividade prática da disciplina de Front-end / PHP.  
Ele aplica conceitos de:
- Orientação a Objetos (OO)
- Relacionamento entre objetos (Produto → Fornecedor)
- Autenticação com senha criptografada (SHA-256)
- CRUD com AJAX
- Banco de Dados MySQL com PDO
- Interface com Bootstrap 5

---

## ✅ Funcionalidades
- **Cadastro de Usuários** com senha em SHA-256  
- **Login e Logout** de usuários  
- **Gerenciamento de Fornecedores** (CRUD via AJAX)  
- **Gerenciamento de Produtos** (CRUD via AJAX, vínculo com Fornecedor)  
- **Cesta de Compras**  
  - Seleção de produtos via checkbox  
  - Validação antes de adicionar  
  - Resumo com **quantidade total** e **valor total**  
  - Botão para **esvaziar a cesta**  
- **Proteção de rotas** e de **APIs** (somente autenticados acessam)

---

## 🗂️ Estrutura do Projeto
mini-produtos/
│
├── app/ # Telas principais (Dashboard, Produtos, Fornecedores, Selecionar, Cesta, Usuários)
│ ├── models/ # Classes OO (Produto, Fornecedor, Usuario)
│ ├── repositories/ # Repositories para acesso ao banco
│ └── partials/ # Navbar, footer e componentes reutilizáveis
│
├── api/ # Endpoints para AJAX
│ ├── produtos/
│ └── fornecedores/
│
├── auth/ # Autenticação (login, registro, logout)
├── config/ # Configurações (db.php, session.php, api_guard.php)
├── database/ # Bootstrap do banco de dados
├── docs/ # Documentos (DER, prints do Figma)
└── README.md # Documentação

---

## 🖥️ Protótipos no Figma
👉 Cole aqui o link do seu Figma  
- Prints estão disponíveis em `/docs/prints/`

---

## 🗺️ Diagrama Entidade-Relacionamento (DER)
Modelo criado no **MySQL Workbench**:  

![DER](docs/der.png)

---

## ⚙️ Como Rodar o Projeto (Windows + XAMPP)
1. Instale o **XAMPP** (Apache + MySQL).  
2. Copie a pasta `mini-produtos` para:  

C:\xampp\htdocs\

3. Inicie **Apache** e **MySQL** no XAMPP.  
4. No navegador, abra:  

http://localhost/mini-produtos/database/bootstrap.php

Isso cria automaticamente o banco de dados e tabelas.  
5. Depois acesse o sistema:  
http://localhost/mini-produtos/
(O `index.php` redireciona para a tela de login).  

---


6. Faça login com o usuário admin criado pelo bootstrap ou registre um novo usuário.
---

## 🛠️ Tecnologias Utilizadas
- PHP 8+  
- MySQL (PDO)  
- HTML5 / CSS3 / JavaScript  
- Bootstrap 5  
- AJAX (fetch API)  

---
