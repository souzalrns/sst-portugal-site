# SST Portugal

> Site institucional para consultoria de segurança e saúde no trabalho, com conteúdo técnico setorial e posicionamento dual advocacia + TSST.

![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)
![HTML](https://img.shields.io/badge/HTML-Estático-e34f26)
![Vercel](https://img.shields.io/badge/Deploy-Vercel-black)

---

## O Problema

Empresas portuguesas precisam de consultoria de segurança no trabalho (SST) juridicamente sólida, mas a maioria dos consultores do setor não tem formação jurídica — e a maioria dos advogados não tem certificação técnica de SST. Este site posiciona a dupla certificação (advogada + Técnica Superior de Segurança no Trabalho) como diferenciador direto para compliance B2B.

## Principais Funcionalidades

- **7 artigos setoriais** de formação (construção civil, indústria fabril, hotelaria/restauração, saúde, comércio/retalho, escritórios, logística/armazenagem)
- **Guia SST** de referência geral
- Site estático, sem dependências de framework — carregamento imediato

## Stack Técnica

- **Frontend:** HTML/CSS estático (sem framework — decisão deliberada, ver abaixo)
- **Infraestrutura:** Vercel

## Destaques Técnicos

1. **Estático por escolha, não por limitação:** sem React/Vue/build step — um site institucional de conteúdo não precisa da complexidade de uma SPA. Menos partes móveis, deploy mais simples, performance de carregamento imediata.
2. **Noindexado até certificação estar completa:** o site fica deliberadamente fora de motores de busca até a certificação TSST (Nível 6) da responsável estar formalmente concluída — evita reivindicar credenciais antes de as ter, uma decisão de integridade profissional refletida em configuração técnica (robots.txt).

## Como Rodar Localmente

Site estático — basta abrir `index.html` num browser, ou servir com qualquer servidor HTTP simples:

```bash
git clone https://github.com/souzalrns/sst-portugal-site.git
cd sst-portugal-site
npx serve .
```

## Estado do Projeto

**Em desenvolvimento** — 7 artigos setoriais publicados, site mantido noindexado até conclusão da certificação TSST Nível 6.

---

Feito por Luiz Souza • [LinkedIn](#) • [Portfólio](#)
