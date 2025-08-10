# PUC_faq-rag
Chatbot de Perguntas Frequentes com RAG (Retrieval-Augmented Generation), usando FAISS para busca vetorial e modelos da Hugging Face. Implementado em Python/Jupyter Notebook como projeto didático para responder FAQs de um domínio específico a partir de documentos locais.

---

# ❄️ RAG Chat Snowboard – Sistema de Perguntas e Respostas

Este projeto implementa um **chat interativo com ipywidgets** para responder perguntas sobre **equipamentos de snowboard** usando a técnica **RAG (Retrieval-Augmented Generation)**.
Ele combina **recuperação de contexto** a partir de um documento técnico com **geração de resposta** via **OpenAI GPT-4o-mini**.

---

## 📌 Funcionalidades

* 🔍 **Busca semântica** usando **FAISS** + embeddings da **Sentence-Transformers**.
* 📄 **Chunking inteligente** do texto com `RecursiveCharacterTextSplitter` e overlap.
* 🤖 **Respostas curtas e naturais** com **prompt otimizado**.
* 🎛 **Interface interativa** com **ipywidgets** para inserir perguntas, ajustar `k` e exibir fontes.
* 🔑 **Leitura automática da API Key** a partir de `config.ini`.
* 🏂 Base de conhecimento: *Guia de Equipamentos de Snowboard*.

---

## ⚙️ Pré-requisitos

* Python 3.10+
* Conta na [OpenAI](https://platform.openai.com/) e chave de API válida
* Ambiente virtual (opcional, mas recomendado)

---

## 🔑 Configuração da API Key

Crie um arquivo `config.ini` na raiz do projeto com o seguinte conteúdo:

```ini
[openai]
api_key = SUA_CHAVE_OPENAI_AQUI
```

---

## ▶️ Execução

Abra o **Jupyter Notebook**:

Na interface:

1. Digite sua pergunta no campo de texto.
2. Ajuste o valor de `k` (número de chunks recuperados).
3. Escolha se deseja **mostrar fontes**.
4. Pressione **Enviar**.

---

## 📄 Exemplo de Uso

**Pergunta:**

```
Quais os tipos de shape de prancha de snowboard?
```

**Resposta:**

```
Os shapes mais comuns são o Directional, ideal para freeride; o Twin, simétrico para freestyle; e o Directional Twin, que combina características dos dois.
```

**Fonte:**

```
guia_equipamentos_snowboard.txt
```

---

## 🛠 Tecnologias Utilizadas

* **[LangChain](https://python.langchain.com/)**
* **[FAISS](https://github.com/facebookresearch/faiss)**
* **[Sentence Transformers](https://www.sbert.net/)**
* **[OpenAI API](https://platform.openai.com/)**
* **[ipywidgets](https://ipywidgets.readthedocs.io/en/latest/)**

---

## 📜 Licença

Este projeto é distribuído sob a licença MIT.
Sinta-se livre para usar, modificar e compartilhar.
