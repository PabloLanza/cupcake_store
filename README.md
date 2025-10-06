#  Cupcake Store — Sistema de Pedidos Online

Sistema web completo para gestão de pedidos de cupcakes, desenvolvido como projeto acadêmico.  
Inclui **front-end (HTML, CSS, JS)** e **back-end (Python + Flask)**, seguindo o **padrão MVC** e com **testes automatizados**.

---

## 🚀 Objetivo
Permitir que clientes realizem pedidos de cupcakes personalizados, acompanhem o status e avaliem suas compras, enquanto funcionários administram pedidos, estoque e relatórios de vendas.

---

##  Tecnologias Utilizadas

### Front-end
- **HTML5** — estrutura das páginas  
- **CSS3** — estilização responsiva  
- **JavaScript (Vanilla)** — interatividade e validação  
- **Jinja2** — renderização de templates pelo Flask  

### Back-end
- **Python 3.10+**  
- **Flask** — microframework web  
- **Flask-SQLAlchemy** — ORM para o banco de dados  
- **SQLite** — banco local simples e portátil  

### Testes
- **pytest** — testes de back-end  
- *(opcional para front-end)* Jest ou Cypress  

---

## 🧱 Arquitetura do Sistema — Padrão MVC

```text
cupcake_store/
├── app.py                → inicialização e registro de rotas (Controllers)
├── config.py             → configuração geral (chaves e banco)
│
├── models/               → camada Model (dados e regras de negócio)
│   ├── user.py
│   ├── product.py
│   ├── order.py
│   └── __all_models__.py
│
├── controllers/          → camada Controller (regras de fluxo e rotas)
│   ├── auth_controller.py
│   ├── product_controller.py
│   ├── order_controller.py
│   └── admin_controller.py
│
├── templates/            → camada View (HTML + Jinja2)
│   ├── base.html
│   ├── login.html
│   ├── register.html
│   ├── menu.html
│   ├── cart.html
│   └── admin_dashboard.html
│
├── static/               → arquivos estáticos (CSS e JS)
│   ├── css/style.css
│   └── js/main.js
│
├── tests/                → testes automatizados (pytest)
│   ├── test_auth.py
│   ├── test_order.py
│   └── conftest.py
│
├── requirements.txt      → dependências do Python
└── database.db           → banco SQLite gerado automaticamente
```

⚙️ Instalação e Execução Local
1️⃣ Clonar o repositório
````
git clone https://github.com/seuusuario/cupcake_store.git
````
Navegue até a pasta 
````
cd cupcake_store
````

2️⃣ Criar e ativar ambiente virtual
````
python -m venv venv
````
# Windows
````
venv\Scripts\activate
````
# Linux/Mac
````
source venv/bin/activate
````

3️⃣ Instalar dependências
````
pip install -r requirements.txt
````

4️⃣ Executar o servidor
````
python app.py
````

Acesse no navegador:

👉 http://127.0.0.1:5000/


🧪 Testes Automatizados
Executar testes com pytest
````
pytest tests -v
````
📋 Exemplos de testes incluídos:

Registro e login de usuário

Criação de pedido

Comunicação entre Controllers e Models

🧰 Estrutura de Banco de Dados (Entidades Principais)
Entidade	Atributos Principais
User	id, name, email, password_hash, role
Product	id, name, description, price, stock
Order	id, user_id, status, total, created_at

(futuras entidades: Review, Coupon, Inventory, Payment)

🧩 Diagrama MVC Simplificado
````
[Usuário] ⇄ (HTML/CSS/JS) ⇄ [Flask Controller] ⇄ [Models/BD]
````
🛠️ Funcionalidades Implementadas
Cliente
Cadastro e login de usuário

Visualização de cardápio

Personalização de cupcake

Adição ao carrinho

Finalização do pedido

Acompanhamento de status

Avaliação e notificações

Funcionário/Admin
Login de funcionário

Atualização de status de pedidos

Gestão de estoque e produtos

Relatórios de vendas

Criação e uso de cupons de desconto

🧱 Design Pattern: MVC (Model-View-Controller)
Camada	Responsabilidade
Model	Estrutura e regras de negócio (User, Product, Order)
View	Interface com o usuário (HTML + CSS + JS via templates)
Controller	Lógica de fluxo, validação, controle de rotas e integração

🧩 Tratamento de Erros
Validação de dados no front-end e back-end

Respostas HTTP adequadas (400, 401, 404, 500)

Mensagens amigáveis ao usuário via flash()

Logs de erro no console (podem ser salvos em arquivo .log)

🧰 Próximos Passos (Versões Futuras)
Autenticação com Flask-Login

Sistema de notificações e e-mail

Testes E2E com Cypress

Deploy no Render ou Railway

🧑‍💻 Autor
Pablo Lanza
Projeto acadêmico — Curso de Engenharia de Software
Cruzeiro do Sul Virtual — 2025

📜 Licença
Uso acadêmico e educacional.
Código aberto para fins de aprendizado e avaliação.
