# 🤖 Assistente de IA com RAG

Projeto desenvolvido com o objetivo de estudar e praticar o conceito de **RAG (Retrieval-Augmented Generation)**, explorando a integração entre inteligência artificial, busca semântica e documentos PDF.

## 🎯 Objetivo

Compreender, na prática, como construir um assistente de IA capaz de responder perguntas com base em informações extraídas de documentos fornecidos, utilizando recuperação de contexto para gerar respostas mais relevantes.

## 🛠️ Tecnologias utilizadas

- **Python** — linguagem de programação.
- **LangChain** — integração e organização do fluxo de processamento da IA.
- **FAISS** — armazenamento e busca vetorial.
- **OpenAI API** — geração de respostas e criação de embeddings.
- **Streamlit** — desenvolvimento da interface interativa.
- **PyPDF** — extração de conteúdo de documentos PDF.

## ⚙️ Como funciona

O sistema utiliza um fluxo RAG dividido nas seguintes etapas:

1. **Carregamento:** extração do texto de um documento PDF.
2. **Divisão em blocos:** fragmentação do conteúdo em partes menores.
3. **Geração de embeddings:** transformação dos blocos de texto em representações vetoriais.
4. **Busca semântica:** recuperação dos trechos mais relevantes para a pergunta do usuário.
5. **Geração de respostas:** envio da pergunta e do contexto recuperado ao modelo de IA.
6. **Exibição:** apresentação da resposta na interface desenvolvida com Streamlit.

## 🚀 Como executar

### 1. Clone o repositório

```bash
git clone <URL_DO_REPOSITORIO>
cd <NOME_DO_REPOSITORIO>
```

### 2. Instale as dependências

Certifique-se de ter Python e pip instalados. Em seguida, execute:

```bash
pip install -r requirements.txt
```

### 3. Configure a API da OpenAI

Crie um arquivo `.env` na raiz do projeto e adicione sua chave de API:

```env
OPENAI_API_KEY=sua_chave_aqui
```

**Importante:** não compartilhe sua chave de API nem envie o arquivo `.env` para o GitHub.

### 4. Adicione o documento PDF

Disponibilize o documento que será utilizado como base de conhecimento, respeitando o nome e o caminho configurados no código.

### 5. Execute a aplicação

```bash
streamlit run app_basico.py
```

Após iniciar, acesse o endereço local exibido no terminal para interagir com o assistente.

## 📚 Aprendizados

Este projeto tem como finalidade consolidar conhecimentos sobre:

- Fundamentos de RAG e geração aumentada por recuperação.
- Processamento e divisão de documentos.
- Embeddings e bancos de dados vetoriais.
- Busca semântica e recuperação de contexto.
- Integração de modelos de linguagem com aplicações Python.
- Desenvolvimento de interfaces interativas com Streamlit.
- Gerenciamento de dependências e variáveis de ambiente.

## 🔮 Possíveis melhorias

- Permitir o envio de diferentes documentos PDF pela interface.
- Implementar histórico de conversas.
- Exibir os trechos e as páginas utilizados para fundamentar cada resposta.
- Melhorar o tratamento de erros e perguntas sem contexto relevante.
- Explorar a disponibilização do assistente por meio de uma API.

---

**Status:** Projeto de estudo em desenvolvimento.

**Propósito:** aprendizado prático de RAG e integração de inteligência artificial com Python.
