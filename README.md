# Zentra — Dashboard Fintech

Projeto desenvolvido para a atividade avaliativa da FIAP ON: **criação das páginas do Fintech** com HTML, CSS e Tailwind CSS, com publicação no GitHub.

## Links

| Recurso | URL |
|--------|-----|
| **Deploy (GitHub Pages)** | https://stwally.github.io/zentra/ |
| **Repositório GitHub** | https://github.com/Stwally/zentra |

> O repositório está **público** para permitir a correção pela plataforma e pelo professor.

---

## Sobre o projeto

**Zentra** é uma fintech fictícia focada em gestão financeira pessoal. Esta entrega contempla **uma tela**: o **dashboard principal**, onde o usuário visualiza um resumo financeiro, métricas em cards e sugestões para interação com um assistente.

A interface segue identidade visual escura (fundo `#0a0a0a`, superfícies `#111111`, bordas `#222222`), tipografia **Inter** para textos de interface e **Playfair Display** para destaques, alinhada ao protótipo da Fase 2.

### Conteúdo da tela

- Saudação e ações rápidas (Adicionar Fundo, Nova Transferência)
- Grid de métricas: saldo, investimentos, resumo semanal, gastos, entradas, evolução, projeção e atualizações
- Bloco de sugestões do assistente financeiro
- Campo para perguntar ao assistente
- Navegação lateral (desktop) e barra inferior (mobile)

---

## Tecnologias utilizadas

- **HTML5** — estrutura semântica (`header`, `main`, `section`, `article`, `nav`, `aside`)
- **CSS3** — estilos customizados em arquivo separado (`global.css`)
- **Tailwind CSS** — layout e utilitários via CDN, com configuração de cores e breakpoints no próprio `index.html`
- **Git / GitHub** — versionamento e deploy via GitHub Pages

Não foi utilizado **JavaScript**, conforme permitido pela atividade.

---

## Estrutura de arquivos

```
zentra/
├── index.html          # Tela principal (abrir este arquivo)
├── global.css          # Estilos globais e componentes (cards .metric)
├── README.md           # Documentação do projeto
└── images/
    ├── fintech_logo.svg
    ├── profile_picture.png
    └── icons/          # Ícones SVG da navegação
```

---

## Como executar na máquina do professor

1. Baixe o repositório ou extraia o **ZIP** da entrega.
2. Abra a pasta do projeto.
3. Dê **duplo clique** em `index.html` ou abra o arquivo no navegador (Chrome, Edge, Firefox).

**Requisitos:** conexão com a internet na primeira abertura (Tailwind CSS e Google Fonts são carregados por CDN).

Não é necessário instalar Node.js nem rodar servidor, desde que os caminhos das imagens (`images/...`) permaneçam na mesma estrutura.

---

## Responsividade

O layout foi pensado para **mobile first**:

- Grid de métricas: 1 coluna no mobile, 2 a partir de `400px` (`xs`), 3 em `lg` e 4 em `xl`
- Menu inferior fixo em telas pequenas; sidebar em `md` (768px) ou superior
- Espaçamentos e tipografia ajustados com breakpoints do Tailwind (`sm`, `md`, `lg`)
- Classes `safe-top` e `safe-bottom` para áreas seguras em dispositivos com notch

---

## Separação HTML e CSS

| Arquivo | Responsabilidade |
|---------|------------------|
| `index.html` | Marcação, conteúdo e classes Tailwind |
| `global.css` | Reset, fontes, safe areas e estilos dos cards de métricas (`.metric`) |

O Tailwind complementa o CSS externo; o projeto **não** concentra toda a estilização em um único arquivo inline.

---

## Identidade visual (padrões)

- **Cores:** `page`, `surface`, `line` (definidas no `tailwind.config`)
- **Tipografia:** Inter (UI) e Playfair Display (títulos)
- **Componentes:** cards com borda uniforme, três primeiros com fundo destacado (`metric--fill`)
- **Ícones e logo:** SVG e PNG na pasta `images/`

---

## Atendimento aos critérios da atividade

| Critério | Peso | Como foi atendido |
|----------|------|-------------------|
| Estrutura e contexto da tela | 20% | Dashboard coerente com proposta Fintech; informações organizadas em seções claras |
| Funcionamento e organização | 20% | Abertura via `index.html`; imagens e CSS no repositório; links relativos |
| Responsividade | 10% | Layout adaptável com Tailwind (grid, sidebar/nav, breakpoints) |
| Separação HTML e CSS | 10% | `index.html` + `global.css` |
| Uso de Tailwind CSS | 10% | CDN + classes utilitárias e tema customizado |
| GitHub e versionamento | 30% | Repositório público + deploy em GitHub Pages |

### Regras da atividade

- [x] Apenas **1 tela** do Fintech
- [x] HTML e CSS em arquivos **separados**
- [x] Sem JavaScript
- [x] Tela relacionada ao projeto Fintech
- [x] Responsividade mobile
- [x] Uso de Tailwind CSS
- [x] Projeto abre pelo arquivo `.html`
- [x] Repositório **público** no GitHub

---

## Autor
Projeto individual — FIAP ON (Fase 4 — Fintech).

GitHub: [@Stwally](https://github.com/Stwally)
