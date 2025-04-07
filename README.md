# 🔍 Azure AI Search para Análise de Notícias

Este projeto demonstra como criar uma solução de busca inteligente usando **Azure Cognitive Search** com dados de um banco de dados **MySQL** contendo notícias.

A solução utiliza **recursos de inteligência artificial (Skillsets)** como:
- Extração de entidades nomeadas (pessoas, locais, organizações)
- Análise de sentimentos dos textos
- Indexação de conteúdo textual

## 🧠 Objetivo

Permitir que usuários façam buscas semânticas em um acervo de notícias, com retorno enriquecido por inteligência artificial.

---

## 🛠️ Tecnologias Utilizadas

- Azure Cognitive Search (Free Tier)
- Banco de dados MySQL (dados de notícias)
- Python (consulta via API REST)
- Azure Skillsets (IA para análise de texto)

---

## 📁 Estrutura do Projeto

azure-news-ai-search/ ├── README.md ├── azure-search-config.json ├── insights.md ├── src/ │ └── consulta-api.py └── screenshots/ └── exemplo.png


---

## 🔧 Como Configurar

### 1. Banco de Dados MySQL

Crie a tabela `noticias`:

```sql
CREATE TABLE noticias (
  id INT PRIMARY KEY,
  titulo VARCHAR(255),
  autor VARCHAR(100),
  data_publicacao DATE,
  conteudo TEXT
);

