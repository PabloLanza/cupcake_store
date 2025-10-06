# 🍰 Cupcake Store

**Cupcake Store** é um sistema web desenvolvido como projeto integrador do curso de Engenharia de Software, cujo objetivo é permitir que clientes personalizem, comprem e acompanhem cupcakes de forma prática e intuitiva.  
O sistema foi construído com base em princípios de **arquitetura MVC** e segue metodologias ágeis, com histórias de usuário detalhadas e priorizadas.

---

## 🚀 Objetivo do Projeto
Desenvolver uma aplicação completa (front-end e back-end) que permita:
- Cadastro e login de usuários.
- Visualização de cardápio e personalização de cupcakes.
- Adição ao carrinho e finalização de pedidos.
- Acompanhamento do status do pedido em tempo real.
- Gestão interna de pedidos, estoque e relatórios de vendas.

---

## 🧩 Arquitetura do Sistema (MVC)

O sistema segue o padrão **Model-View-Controller (MVC)**:

/cupcake-store
├── frontend/ # Interface do usuário (HTML, CSS, JS)
├── backend/ # Regras de negócio e integração com o banco
│ ├── controllers/ # Lógica de controle (cadastro, login, pedidos)
│ ├── models/ # Classes e estruturas de dados
│ ├── views/ # Respostas e renderizações
│ └── app.py # Ponto principal da aplicação
├── tests/ # Testes unitários e de integração
├── docs/ # Documentação e relatórios de validação
└── README.md # Este arquivo

yaml
Copiar código

---

## 🛠️ Tecnologias Utilizadas

| Camada | Tecnologias | Função |
|--------|--------------|--------|
| **Front-end** | HTML5, CSS3, JavaScript | Interface do usuário |
| **Back-end** | Python + Flask | Lógica, rotas e controle de dados |
| **Banco de Dados** | SQLite | Armazenamento local de dados |
| **Testes** | PyTest | Testes unitários e de integração |
| **Versionamento** | Git + GitHub | Controle de versão e publicação |
| **Design Pattern** | MVC | Organização e desacoplamento de componentes |

---

### 🔹 Passos para executar

# Clonar o repositório
````
git clone https://github.com/seuusuario/cupcake-store.git
````
# Acessar o diretório
````
cd cupcake-store/backend
````

# Criar e ativar ambiente virtual
````
python -m venv venv
source venv/bin/activate  # (no Windows: venv\Scripts\activate)
````
# Instalar dependências
pip install flask pytest
````
# Executar a aplicação
python app.py
````
Acesse no navegador:
➡️ http://localhost:5000

🧪 Testes
Os testes são realizados com PyTest para garantir a confiabilidade das funções principais.

# Executar testes
````
pytest tests/
````
Os testes cobrem:

Cadastro e login de usuários

Criação e atualização de pedidos

Atualização de status e controle de estoque

Validação de regras de negócio

🗂️ Estrutura de Diretórios
````pgsql
/cupcake-store
├── frontend/
│   ├── index.html
│   ├── login.html
│   ├── cadastro.html
│   ├── carrinho.html
│   └── styles/
│       └── style.css
├── backend/
│   ├── app.py
│   ├── controllers/
│   ├── models/
│   └── views/
├── tests/
│   └── test_app.py
├── docs/
│   ├── testes.md
│   ├── feedbacks/
│   └── prints/
└── README.md
````

👥 Autoria
Aluno: Pablo Lanza
Curso: Engenharia de Software — Cruzeiro do Sul Virtual
Disciplina: Projeto Integrador Transdisciplinar II

📄 Licença
Este projeto é de uso acadêmico e pode ser utilizado como portfólio pessoal.
© 2025 — Todos os direitos reservados.
