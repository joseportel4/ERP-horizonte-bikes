# Horizonte Bikes — ERP

Sistema Integrado de Gestão (**ERP + Business Intelligence**) para **Bike Shop & Oficina**.

## Tecnologias

- **Linguagem:** Python 3.11+
- **Interface Web:** Streamlit
- **Banco de Dados:** PostgreSQL (Supabase)
- **ORM & Validação:** SQLAlchemy 2.0 + Pydantic v2
- **Autenticação:** Google OAuth 2.0 / OIDC
- **Análise & BI:** Pandas + Plotly
- **Comprovantes:** FPDF2

## Estrutura do Projeto

```text
ERP-horizonte-bikes/
├── .streamlit/              # Configurações e template de segredos do Streamlit
├── docs/                    # Documentação técnica e requisitos da disciplina
├── sql/                     # Scripts SQL (DDL, views analíticas, seeds)
├── src/
│   ├── config/              # Configurações gerais, banco de dados e autenticação
│   ├── models/              # Entidades ORM (SQLAlchemy)
│   ├── schemas/             # Schemas de validação (Pydantic)
│   ├── repositories/        # Camada de persistência e consultas
│   ├── services/            # Regras de negócio e integração entre módulos
│   ├── ui/                  # Interface Streamlit (pages e components)
│   └── utils/               # Utilitários gerais (formatação, PDF, etc.)
├── tests/                   # Testes automatizados (Pytest)
├── app.py                   # Ponto de entrada da aplicação Streamlit
└── requirements.txt         # Dependências do projeto
```

## Execução Local

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
streamlit run app.py
```
