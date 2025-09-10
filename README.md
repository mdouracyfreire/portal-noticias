# 📰 Portal de Notícias — Prática de Grid Layout (Rocketseat)

Este projeto é uma **atividade prática** do módulo **Grid Layout** do curso **Fullstack** da [Rocketseat](https://www.rocketseat.com.br/). O objetivo do desafio foi criar uma página de notícias responsiva, usando **CSS Grid** como principal ferramenta de layout, organizando o código em arquivos CSS modulares e reutilizáveis.

---

## 🎯 Objetivo

- Praticar conceitos de **CSS Grid** aplicados a um layout real de portal de notícias.  
- Separar responsabilidades em arquivos CSS (global, seção, cabeçalho, utilitários).  

---

## 🎥 Demonstração


**Tela principal:**

![Image](https://github.com/user-attachments/assets/5de1bd29-c531-41bd-91ac-723f0ac4e11e)

---

## 🛠 Tecnologias utilizadas

- **HTML5** (estrutura semântica)  
- **CSS3** (CSS Grid, Flexbox, Media Queries, variáveis CSS)  
- **Google Fonts** (Archivo, Vollkorn)  
- Abordagem **utility-first** para classes reutilizáveis

---

## 📂 Estrutura do projeto (baseada nos arquivos enviados)

```
/ (raiz do projeto)
├── index.html
├── assets/
│   ├── Logo.svg
│   ├── Ads.png
│   ├── icons/
│   │   ├── List.svg
│   │   ├── MagnifyingGlass.svg
│   │   ├── ArrowRight.svg
│   │   └── ArrowRight-hover.svg
│   ├── images/
│       ├── Image 01.png
│       ├── Image 02.png
│       ├── Image 03.png
│       └── ... (Image 04.png → Image 18.png)
└── styles/
    ├── index.css                 # ponto de entrada (importa os demais arquivos CSS)
    ├── global.css                # variáveis, reset e estilos base (cores, fontes, container)
    ├── header.css                # estilos do header primário (#primary) e secundário (#secondary)
    ├── section.css               # estilos das seções (featured, weekly, ai, aside, more)
    └── utility.css               # classes utilitárias (grid helpers, gaps, tipografia)
```

**Observações sobre a estrutura:**  
- O HTML referencia o arquivo `./styles/index.css`, que serve como ponto único para importar ou concatenar os demais arquivos CSS.  
- A pasta `assets/` contém ícones, imagens de destaque e possíveis GIFs para demonstração.  

---

## 📌 Organização dos estilos (resumo)

- **index.css** — Arquivo principal que carrega/encadeia os outros arquivos de estilo. Mantém o ponto único de importação no HTML.  
- **global.css** — Contém: reset (`* { box-sizing, margin, padding }`), variáveis CSS (`:root`), tipografia, cores, `.container` e regras base do layout.  
- **header.css** — Controla o layout do cabeçalho: grid/flex para posicionar menu, logo e busca; estilos do menu secundário com bordas e espaçamento.  
- **section.css** — Estilos específicos das seções: cards em destaque com gradiente, posicionamento de `content-tag`, grids das listas “Mais lidas” e blocos de artigos em destaque. Utiliza seletores modernos (`:has`, pseudo-elementos e `::before`) para efeitos visuais.  
- **utility.css** — Conjunto de utilitários (ex.: `.grid`, `.grid-flow-col`, `.grid-cols-2`, `.gap-16`, `.text-2xl`) para acelerar o desenvolvimento e reduzir repetição de código.

---

## 🚀 Como visualizar localmente

1. Faça o clone do repositório:
```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
```

2. Entre na pasta do projeto:
```bash
cd seu-repositorio
```

3. Abra `index.html` no navegador ou use uma extensão como **Live Server** (VS Code) para desenvolvimento com reload automático.

---

## ✅ Boas práticas implementadas / aprendizados

- Modularização dos estilos em arquivos com responsabilidades claras.  
- Reuso por meio de classes utilitárias (reduz duplicação).  
- Uso de `:root` para centralizar tokens de design (cores, tipografia).  
- Aplicação prática de CSS Grid para layouts complexos.  

---

## ✨ Autor

Projeto desenvolvido por **[Douracy Freire](https://github.com/mdouracyfreire)**

---

> Este projeto é uma atividade prática do módulo de Grid Layout para fins de estudo e portfólio.
