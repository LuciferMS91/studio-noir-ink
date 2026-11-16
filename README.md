# NOIR INK Studio — Tattoo & Piercing

Website institucional e editorial desenvolvido para o **NOIR INK Studio**, um estúdio fictício dedicado à arte da tatuagem, body piercing, projetos personalizados e fornecimento de insumos profissionais.

🔗 **Acesse o projeto online:** [luciferms91.github.io/studio-noir-ink](https://luciferms91.github.io/studio-noir-ink/)

---

## Sobre o Projeto

O projeto foi construído **100% em HTML5 e CSS3 puros** (sem frameworks ou JavaScript), com foco em estética editorial, tipografia clássica, responsividade completa para dispositivos móveis e arquitetura de código limpa e modular.

### Identidade Visual
* **Paleta de Cores:** Contraste sofisticado entre fundo escuro (`#0A0A0A`), superfícies em grafite (`#1C1C1C`) e detalhes em dourado metálico (`#D4AF37`).
* **Tipografia:** Combinação da fonte romana **Cinzel** (Google Fonts) para títulos e logotipo com **Segoe UI / Roboto** para leitura fluida nos textos.

---

## Páginas e Funcionalidades

O site é composto por **10 páginas HTML interligadas** com navegação consistente:

1. **Início (`index.html`):** Apresentação do estúdio, destaques, prévia da galeria, serviços, depoimentos de clientes e informações de contato rápido.
2. **Galeria (`html/galeria.html`):** Grade assimétrica (*CSS Grid*) exibindo trabalhos de tatuagem, fine line, realismo e joalheria.
3. **Piercings (`html/piercings.html`):** Guia de perfurações, catálogo de joias (Labret, Barbell, Argola, CBR), etapas do procedimento e cuidados pós-perfuração.
4. **Equipe (`html/equipe.html`):** Apresentação dos tatuadores e body piercers, suas especialidades e filosofias de trabalho.
5. **Estúdio (`html/estudio.html`):** Tour visual pelos ambientes do estúdio (recepção, salas de tatuagem, sala de piercing e vitrine de joias).
6. **Agendamento (`html/agendamento.html`):** Formulário interativo em etapas para escolha de serviço, seleção visual de profissional (com cards selecionáveis em CSS puro usando `:has(:checked)`), data e horário.
7. **Serviços (`html/servicos.html`):** Banners de serviços e **carrossel interativo de catálogo de insumos** construído exclusivamente com CSS puro (utilizando pseudo-classes `:target` e `:has()`).
8. **Contato (`html/contato.html`):** Canais de atendimento direto (WhatsApp, E-mail e Instagram), formulário de mensagem e localização.
9. **Confirmação de Agendamento (`html/confirmacao.html`):** Página dedicada ao feedback visual exibida após o envio do formulário de agendamento.
10. **Mensagem Enviada (`html/mensagem-enviada.html`):** Página dedicada a confirmação exibida após o envio do formulário de contato.

---

## Destaques Técnicos

* **Arquitetura CSS Modular (`global.css` e `confirmacao-style.css`):** Centralização de variáveis (`:root`), reset, tipografia base, cabeçalho fixo (`sticky`), menu de navegação e rodapé no `global.css`, além do reaproveitamento do `confirmacao-style.css` entre as telas de feedback, eliminando duplicação de código.
* **Organização Visual:** Arquivos CSS específicos organizados de cima para baixo espelhando exatamente a estrutura semântica do HTML.
* **Interatividade sem JavaScript:** Uso avançado de seletores modernos de CSS (`:target`, `:has()`, `counter-reset`) para carrossel de produtos, seleção de cards de profissionais e listas numeradas estilizadas.
* **Acessibilidade e Semântica:** Uso de tags semânticas (`header`, `nav`, `main`, `section`, `article`, `figure`, `blockquote`, `footer`), atributos ARIA (`aria-current="page"`, `aria-labelledby`, `aria-hidden`) e estados de foco visíveis (`:focus-visible`).
* **Favicon em SVG Embutido:** Ícone vetorial com o monograma **NI** codificado diretamente em Base64 no `<head>` de todas as páginas.

---

## Estrutura de Pastas

```
studio-noir-ink/
├── index.html
├── README.md
├── css/
│   ├── agendamento-style.css
│   ├── confirmacao-style.css
│   ├── contato-style.css
│   ├── equipe-style.css
│   ├── estudio-style.css
│   ├── galeria-style.css
│   ├── global.css
│   ├── index-style.css
│   ├── piercings-style.css
│   └── servicos-style.css
├── html/
│   ├── agendamento.html
│   ├── confirmacao.html
│   ├── contato.html
│   ├── equipe.html
│   ├── estudio.html
│   ├── galeria.html
│   ├── mensagem-enviada.html
│   ├── piercings.html
│   └── servicos.html
└── media/
    └── images/
```

## Como Executar Localmente

1. Clone este repositório:
   ```bash
   git clone https://github.com
   ```
2. Abra a pasta do projeto no **Visual Studio Code**.
3. Utilize a extensão **Live Server** (clique em *Go Live*) ou abra o arquivo `index.html` diretamente no navegador.