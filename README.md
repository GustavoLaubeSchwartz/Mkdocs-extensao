# Extensão MkDocs

Este repositório contém o material criado para a disciplina de Extensão do IFES Campus Serra, organizado em um site gerado com **MkDocs + Material for MkDocs**.

O site é um ambiente de apoio para resolução de exercícios e conteúdos apresentados nas aulas.

## Estrutura do projeto

- `extensao/docs/` - Conteúdo em Markdown utilizado para gerar o site.
- `extensao/mkdocs.yml` - Configuração do MkDocs (tema, navegação, plugins, etc.).
- `extensao/site/` - Saída gerada pelo MkDocs (não comitada normalmente, gerada em `mkdocs build`).
- `gh-pages` - Branch usado para publicação no GitHub Pages.

## Como rodar localmente

1. Clone o repositório:

   ```bash
   git clone https://github.com/GustavoLaubeSchwartz/Mkdocs-extensao.git
   cd Mkdocs-extensao/extensao
   ```

2. Crie e ative um ambiente virtual (recomendado):

   ```bash
   python -m venv venv
   # Windows
   venv\Scripts\activate
   # Linux / macOS
   # source venv/bin/activate
   ```

3. Instale as dependências:

   ```bash
   pip install mkdocs-material
   ```

4. Rode o servidor local (modo desenvolvimento):

   ```bash
   mkdocs serve
   ```

   Depois acesse: http://127.0.0.1:8000

## Como publicar no GitHub Pages

A publicação é feita automaticamente com o comando abaixo (gerando o site e fazendo deploy para o branch `gh-pages`):

```bash
mkdocs gh-deploy --force
```

## Nota

Este repositório é um **ambiente de suporte** para as atividades da disciplina de Extensão no IFES Campus Serra. O conteúdo principal está em `extensao/docs/` e as aulas são organizadas como páginas Markdown.
