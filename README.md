# langchain-course

Este projeto demonstra o uso da biblioteca LangChain para criar uma cadeia de prompts que resume informações sobre uma pessoa, utilizando modelos de linguagem como o Ollama ou OpenAI.

## Descrição

O script principal (`main.py`) utiliza o LangChain para:
- Receber um texto informativo sobre uma pessoa (no exemplo, Elon Musk).
- Gerar um resumo curto e dois fatos interessantes sobre essa pessoa, usando um modelo de linguagem.
- Exibir o resultado no terminal.

## Requisitos

- Python >= 3.13
- As dependências listadas em `pyproject.toml`:
  - langchain
  - langchain-ollama
  - langchain-openai
  - python-dotenv
  - black, isort (para formatação de código)

## Instalação

1. Clone o repositório:
   ```bash
   git clone <url-do-repositorio>
   cd langchain-course
   ```

2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
   Ou, se estiver usando poetry/pdm, siga o gerenciador de pacotes correspondente.

3. Configure as variáveis de ambiente necessárias em um arquivo `.env` (por exemplo, chaves de API para OpenAI, se for usar).

## Uso

Execute o script principal:
```bash
python main.py
```

O resultado será impresso no terminal, contendo o resumo e fatos interessantes sobre a pessoa definida no código.

## Observações

- O modelo padrão utilizado é o `gpt-oss:20b` via Ollama, mas pode ser facilmente alterado para OpenAI (descomente a linha correspondente no código).
- O projeto serve como base para estudos e experimentação com LangChain e LLMs.
