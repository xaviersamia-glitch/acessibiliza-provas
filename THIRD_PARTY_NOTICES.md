# Bibliotecas de terceiros

Este projeto inclui, sem modificações funcionais, as seguintes bibliotecas na raiz do repositório:

| Biblioteca | Versão | Uso | Licença | Projeto |
|---|---|---|---|---|
| docx | 9.8.1 | Geração dos arquivos Word | MIT | https://github.com/dolanmiu/docx |
| JSZip | 3.10.1 | Leitura de equações em arquivos Word | MIT ou GPL-3.0 (uso sob MIT) | https://github.com/Stuk/jszip |
| mammoth | 1.8.0 | Importação de arquivos Word | BSD-2-Clause | https://github.com/mwilliamson/mammoth.js |
| PDF.js (pdfjs-dist) | 6.2.108 | Importação de arquivos PDF | Apache-2.0 | https://github.com/mozilla/pdf.js |

Nos arquivos `pdf.mjs` e `pdf.worker.mjs`, a instrução final de exportação de módulo foi substituída por uma atribuição a `globalThis`, para permitir o uso sem empacotador.

As fontes Atkinson Hyperlegible e Literata são carregadas do Google Fonts (SIL Open Font License).
