# Learning Log 📚

**Learning Log** é uma aplicação web que permite aos usuários registrar e acompanhar seu aprendizado em diversos tópicos. Com a aplicação, os usuários podem se cadastrar, fazer login e criar tópicos sobre qualquer assunto de interesse, além de adicionar e editar anotações relacionadas ao seu aprendizado. O projeto foi desenvolvido utilizando o framework Django, a linguagem Python e o framework Bootstrap para estilização.

## Funcionalidades

- **Cadastro de Usuários**: Permite que novos usuários se registrem para utilizar o sistema.
- **Login e Logout**: Sistema de autenticação para que os usuários possam acessar seus tópicos e anotações.
- **Criação de Tópicos**: Usuários podem criar tópicos relacionados a diferentes áreas de estudo ou interesses.
- **Adição de Anotações**: Cada tópico pode conter várias anotações para registrar o progresso do usuário.
- **Edição de Anotações**: As anotações podem ser atualizadas a qualquer momento.
- **Interface Responsiva**: A aplicação é estilizada com Bootstrap, garantindo responsividade e compatibilidade com diferentes dispositivos.
---
## Requisitos

- Python 3.8+
- Django 3.0+
- Bootstrap 4 ou 5 (configurado via templates)
- Banco de dados SQLite (ou outro de sua escolha)
---
## Instalação

Siga os passos abaixo para instalar e configurar o projeto localmente:

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/seu-usuario/learning-log.git
   cd learning-log
   ```

2. **Crie e ative um ambiente virtual:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate  # Windows
   ```

3. **Instale as dependências:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Execute as migrações do banco de dados:**
   ```bash
   python manage.py migrate
   ```

5. **Crie um superusuário (administrador):**
   ```bash
   python manage.py createsuperuser
   ```

6. **Inicie o servidor de desenvolvimento:**
   ```bash
   python manage.py runserver
   ```

7. Acesse a aplicação em [http://localhost:8000](http://localhost:8000).
---
## Configuração do Banco de Dados

<p>Por padrão, o projeto utiliza SQLite. Para trocar de banco de dados (MySQL, PostgreSQL, etc.), ajuste o arquivo `settings.py` conforme sua preferência.</p>

---

## Como Usar

### Fluxo de Uso:

1. **Cadastro e Login**:
   - Os usuários devem se registrar na aplicação para criar e gerenciar tópicos e anotações. Após o cadastro, é necessário realizar login para acessar suas funcionalidades.

2. **Criação de Tópicos**:
   - Uma vez logado, o usuário pode criar novos tópicos de estudo, adicionando um título descritivo.

3. **Anotações**:
   - Cada tópico pode ter várias anotações. O usuário pode adicionar conteúdo sobre o que aprendeu e editá-lo posteriormente, se necessário.

4. **Administração**:
   - Um superusuário pode acessar o painel administrativo do Django em `/admin/` para gerenciar usuários e conteúdos.
---
## Tecnologias Utilizadas

- **Django**: Framework web em Python para o backend e gerenciamento de banco de dados.
- **Python**: Linguagem de programação utilizada para toda a lógica da aplicação.
- **Bootstrap**: Framework CSS para estilização e responsividade.
- **SQLite**: Banco de dados padrão do Django (pode ser alterado conforme necessidade).
- **HTML5/CSS3**: Estruturação e estilização das páginas.