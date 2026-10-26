# Acessibiliza Provas

Proposta de ferramenta de apoio ao **Atendimento Educacional Especializado (AEE)** e ao **Núcleo de Atendimento às Pessoas com Necessidades Específicas (NAPNE)** do Colégio Pedro II para a adaptação de avaliações de estudantes com necessidades específicas.

A aplicação funciona inteiramente no navegador, sem servidor e sem cadastro. O docente importa a prova, define o tipo de adaptação e exporta a versão adaptada em Word.

## Funcionalidades

- Importação de provas em **Word (.docx)**, com imagens, tabelas, índices, expoentes e equações do editor do Word; em **PDF** (texto) e por colagem de texto.
- Identificação automática de questões e alternativas, com indicadores de pontos de atenção (enunciado longo, mais de um comando, comando negativo, imagens, tabelas e fórmulas).
- Aplicação dos **quatro tipos de prova adaptada** previstos nas orientações do NAPNE.
- Registro de **barreiras observadas**, sem nome nem diagnóstico, com as estratégias correspondentes do e-book *Educação inclusiva na prática*.
- Regras automáticas: destaque de verbos de comando e negações, separação de comandos e redução de alternativas.
- Uso de inteligência artificial em modo prompt (ChatGPT, Claude ou Gemini), com comandos que já incluem as orientações institucionais.
- Barra de símbolos para **Matemática, Física e Química**, com índices e expoentes.
- Recursos para **estudantes cegos ou com baixa visão**: descrição de imagens e gráficos, tabelas em texto linear e imagens ampliadas.
- Exportação da **prova adaptada** e da **ficha de orientações de aplicação** em .docx, além do arquivo de projeto (.json).

## Guia de uso

O guia completo para docentes está em [`Guia_de_uso_Acessibiliza_Provas.pdf`](Guia_de_uso_Acessibiliza_Provas.pdf).

## Estrutura

Todos os arquivos ficam na raiz do repositório:

```
index.html                 página principal
app.css                    estilos
app.js                     lógica da aplicação
brasao.png                 brasão do Colégio Pedro II
docx.iife.js               geração de arquivos Word
jszip.min.js               leitura de equações em arquivos Word
mammoth.browser.min.js     importação de arquivos Word
pdf.mjs, pdf.worker.mjs    importação de arquivos PDF
Guia_de_uso_Acessibiliza_Provas.pdf
```

## Publicação e atualização

O site é publicado pelo GitHub Pages a partir da branch `main`, pasta raiz (**Settings → Pages**). Para atualizar, use **Add file → Upload files** e envie os arquivos alterados; o GitHub substitui os arquivos com o mesmo nome.

## Privacidade

- A prova é processada no navegador; nenhum dado é enviado a servidor da ferramenta.
- O rascunho fica salvo apenas no navegador do computador em uso.
- Não devem ser registrados nome, matrícula, laudo ou diagnóstico do estudante.
- Ao usar inteligência artificial externa, somente o texto (e, se solicitado, a imagem) é colado pelo próprio docente na ferramenta escolhida.

## Referências pedagógicas

- Colégio Pedro II. NAPNE. *Orientações gerais para adaptações de materiais e avaliações de estudantes com necessidades específicas.*
- THOMÉ, Monique Ferreira Guedes; FORTUNATO, Francisca Sâmia Xavier. *Educação inclusiva na prática: um guia para professores.*
- BRASIL. Lei nº 13.146/2015 (Lei Brasileira de Inclusão).

As orientações são norteadoras. O docente mantém autonomia para decidir o tipo e o modo de adaptação, e a ferramenta não substitui o PEI nem a análise pedagógica.

## Aviso

Esta é uma proposta de ferramenta de apoio elaborada por docente do AEE e não constitui sistema oficial do Colégio Pedro II. O brasão do Colégio Pedro II pertence à instituição e é utilizado apenas para identificação do contexto de uso.

## Autoria

Profa. Francisca Sâmia Xavier Fortunato · Atendimento Educacional Especializado (AEE) · Colégio Pedro II.

## Bibliotecas de terceiros

As bibliotecas de terceiros incluídas no repositório e suas licenças estão listadas em [`THIRD_PARTY_NOTICES.md`](THIRD_PARTY_NOTICES.md).
