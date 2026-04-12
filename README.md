# 🚀 NerdTechShop - Auditoria de Qualidade & Performance

![QA Badge](https://img.shields.io/badge/Status-Estudo-green)
![Gherkin Badge](https://img.shields.io/badge/Language-Gherkin-orange)
![EBAC Badge](https://img.shields.io/badge/Origin-EBAC-blue)
![Lighthouse Score](https://img.shields.io/badge/Lighthouse-Audited-orange)
![HTML Badge](https://img.shields.io/badge/Language-HTML-red)
![CSS Badge](https://img.shields.io/badge/Language-CSS-blueviolet)

Este projeto consiste em uma plataforma básica de e-commerce criada por mim (somente com o intuito de realizar o exercicio) focada no público entusiasta de tecnologia e hardware. O repositório contém o código-fonte da aplicação e um relatório detalhado de auditoria focado em **Acessibilidade**, **Performance** e **UX**.

## 📋 Sobre o Projeto
Meu site apresenta um catálogo de produtos, sistema de busca e banners promocionais. Esta análise foi realizada para identificar gargalos que prejudicam a velocidade de carregamento e impedem o uso por pessoas com necessidades especiais, simulando um cenário real de auditoria de software.

## 🛠️ Metodologia e Ferramentas
A auditoria seguiu rigorosos padrões de mercado, utilizando:
* **Google Lighthouse:** Diagnóstico de Core Web Vitals, SEO e Acessibilidade.
* **Inspeção de Código:** Revisão manual de HTML/CSS via VS Code para identificação de redundâncias e má prática de semântica.
* **Simulação de Redes:** Testes simulando dispositivos móveis (Throttle) e latência de rede instável para validar a resiliência da aplicação.

## 🔍 Principais Achados (Bug Reports)

### 1. Performance: Payload de Imagens Crítico
* **ID:** `Bug-Desempenho001`
* **Problema:** O site carrega um payload de rede de **8.795 KiB**, devido a imagens em resoluções excessivas e formatos não otimizados.
* **Impacto:** Lentidão extrema em dispositivos móveis e maior consumo de dados do usuário.

### 2. Estabilidade Visual: Layout Shift (CLS)
* **ID:** `Bug-Desempenho003`
* **Problema:** Ausência de atributos `width` e `height` em 13 elementos de imagem.
* **Impacto:** Conteúdo "balançando" (Layout Shift) durante o carregamento, gerando uma experiência de navegação frustrante.

### 3. Acessibilidade e Bloqueio de Renderização
* **ID:** `Bug-Desempenho002`
* **Problema:** Recursos de terceiros (Google Fonts/CDN) bloqueando a renderização inicial por **510ms**.
* **Sugestão:** Implementação de fontes de fallback e otimização de contraste para conformidade com o nível **WCAG AA**.

## 📈 Conclusão Técnica
O site apresenta uma base estrutural sólida (semântica de títulos e botões), mas ainda está distante do nível **AAA** de acessibilidade. As melhorias prioritárias focam na **Otimização de Imagens** e **Correção de Contraste** para garantir uma navegação inclusiva, rápida e profissional.

## 💡 Sugestões de Melhoria (Roadmap)
* **Migração para WebP:** Redução de até 80% no peso das imagens sem perda de qualidade visual.
* **Skeleton Screens:** Melhoria da percepção de velocidade através de placeholders de carregamento.
* **Dark Mode Nativo:** Implementação de variação de CSS para conforto visual e economia de bateria em telas OLED.

## 📂 Estrutura do Repositório
* `/Códigos`: Arquivos fonte do projeto (HTML, CSS, JS).
* `/Docs`: Itens usados na estrutura do site.
* `/Evidencias`: Capturas de tela dos diagnósticos e evidências de bugs.
* `/Reports`: Relatório completo de auditoria em PDF.
* `/Sug-alteralçõesviaDevTools`: Parte 2 do exercicío com as alterações via DevTools.
---
**Autor:** [Rodrigo Lins](https://github.com/SEU-USUARIO-AQUI)  
*Analista de QA em transição de carreira | Gestão de TI*
