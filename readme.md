# 🎓 Imersão DevOps - Alura + Google Cloud ☁️

Este projeto é uma **API REST desenvolvida com FastAPI** para gerenciar **alunos**, **cursos** e **matrículas** de uma instituição de ensino.

---

## 🚀 Tecnologias Utilizadas

- 🐍 Python 3.10+
- ⚡ FastAPI
- 🐘 SQLAlchemy + SQLite
- 🐳 Docker
- 🧪 Pydantic
- 🌐 Google Cloud Run

---

## 🧰 Pré-requisitos

Antes de começar, certifique-se de ter instalado:

- [✅ Python 3.10 ou superior](https://www.python.org/downloads/)
- [✅ Git](https://git-scm.com/downloads)
- [✅ Docker](https://www.docker.com/get-started)

---

## 📦 Como rodar o projeto localmente

1. **📥 Clone ou baixe o repositório:**

```bash
git clone https://github.com/rafaelflorentinobarbosa/ellis.git
# ou baixe o ZIP:
# https://github.com/rafaelflorentinobarbosa/ellis/archive/refs/heads/main.zip
```

2. **🐍 Crie um ambiente virtual:**

```bash
python3 -m venv venv
```

3. **▶️ Ative o ambiente virtual:**

- No **Linux/Mac**:
  ```bash
  source venv/bin/activate
  ```

- No **Windows** (modo administrador ou PowerShell):
  ```powershell
  Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
  .\venv\Scripts\activate
  ```

4. **📦 Instale as dependências:**

```bash
pip install -r requirements.txt
```

5. **🏃 Execute a aplicação:**

```bash
uvicorn app:app --reload
```

6. **🧪 Acesse a documentação interativa:**

Abra seu navegador em:

👉 [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

---

## ☁️ Deploy com Google Cloud

Autentique-se e faça o deploy na Cloud Run:

```bash
gcloud auth login
gcloud config set project PROJECT_ID
gcloud run deploy --port=8000
```

---

## 🗂️ Estrutura do Projeto

```
ellis/
├── app.py             # Arquivo principal da aplicação
├── models.py          # Modelos de dados (SQLAlchemy)
├── schemas.py         # Schemas de validação (Pydantic)
├── database.py        # Configuração do banco SQLite
├── routers/           # Rotas organizadas por funcionalidade
│   ├── alunos.py
│   ├── cursos.py
│   └── matriculas.py
├── requirements.txt   # Dependências do projeto
```

📌 O banco `escola.db` é criado automaticamente na primeira execução.

🗑️ Para limpar os dados, basta apagar o arquivo `escola.db`.

---

## 👤 Autor

Desenvolvido por **Rafael Florentino Barbosa**  
📧 [rafaelflorentinobarbosa@gmail.com](mailto:rafaelflorentinobarbosa@gmail.com)  
🔗 [linkedin.com/in/rafaelflorentinobarbosa](https://www.linkedin.com/in/rafaelflorentinobarbosa/)