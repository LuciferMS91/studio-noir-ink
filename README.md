# NOIR INK Studio — Tattoo & Piercing

Website institucional e editorial desenvolvido para o **NOIR INK Studio**, um estúdio fictício dedicado à arte da tatuagem, body piercing, projetos personalizados e fornecimento de insumos profissionais.

🔗 **Acesse o projeto online:** [luciferms91.github.io/studio-noir-ink](https://github.io)

---

## Sobre o Projeto

O projeto foi construído **100% em HTML5 e CSS3 puros** (sem frameworks ou JavaScript), com foco em estética editorial, tipografia clássica, responsividade completa para dispositivos móveis e arquitetura de código limpa, escalável e modular.

### Identidade Visual
* **Paleta de Cores:** Contraste sofisticado entre fundo escuro (`#0A0A0A`), superfícies em grafite (`#1C1C1C`), bordas sutis (`#555555`) e detalhes em dourado metálico (`#D4AF37`).
* **Tipografia:** Combinação da fonte romana **Cinzel** (Google Fonts, com pré-conexão `preconnect`) para títulos e logotipo, aliada à família **Segoe UI / Roboto** para leitura fluida nos textos e formulários.

---

## Páginas e Funcionalidades

O site é composto por **10 páginas HTML interligadas** com navegação consistente e feedback completo ao usuário:

1. **Início (`index.html`):** Capa editorial (*hero*), destaques dos serviços, prévia da galeria, depoimentos de clientes e informações de contato rápido com ícones vetoriais.
2. **Galeria (`html/galeria.html`):** Grade assimétrica (*CSS Grid*) exibindo trabalhos de tatuagem, fine line, realismo e joalheria.
3. **Piercings (`html/piercings.html`):** Guia de perfurações, catálogo de joias (Labret, Barbell, Argola, CBR), etapas do procedimento numeradas via CSS e cuidados pós-perfuração.
4. **Equipe (`html/equipe.html`):** Apresentação dos tatuadores e body piercers, suas especialidades, citações e filosofias de trabalho.
6. **Estúdio (`html/estudio.html`):** Tour visual pelos ambientes do estúdio (recepção, salas de tatuagem, sala de piercing, galeria industrial e vitrine de joias).
6. **Agendamento (`html/agendamento.html`):** Formulário interativo em etapas para escolha de serviço, seleção visual de profissional (com cards interativos em CSS puro), data e horário.
7. **Serviços (`html/servicos.html`):** Banners de serviços e **carrossel interativo de catálogo de insumos** construído exclusivamente com CSS puro.
8. **Contato (`html/contato.html`):** Canais de atendimento direto (WhatsApp, E-mail e Instagram), formulário de mensagem e localização no Google Maps.
9. **Confirmação de Agendamento (`html/confirmacao.html`):** Página dedicada de feedback visual exibida após o envio do formulário de agendamento.
10. **Mensagem Enviada (`html/mensagem-enviada.html`):** Página dedicada de confirmação exibida após o envio do formulário de contato.

---

## Destaques Técnicos e Arquitetura

* **Arquitetura CSS Modular (`global.css` e `confirmacao-style.css`):** Centralização de variáveis (`:root`), reset, tipografia base, cabeçalho fixo (`sticky`), menu de navegação e rodapé no `global.css`, além do reaproveitamento do `confirmacao-style.css` entre as telas de confirmação, eliminando duplicação de código.
* **Organização Espelhada:** Todos os arquivos CSS específicos seguem exatamente a ordem visual de cima para baixo da árvore semântica do HTML, facilitando a leitura e a manutenção.
* **Interatividade sem JavaScript:** Uso de seletores modernos de CSS (`:target`, `:has()`, `counter-reset`) para controlar o carrossel de produtos em 4 grupos, destacar o card do profissional selecionado (`:has(input[type="radio"]:checked)`) e gerar listas numeradas customizadas.
* **Responsividade Mobile-First/Adaptativa:** Media queries (`@media (max-width: 768px)`) que reorganizam grades para coluna única, ajustam tipografia, ocultam divisórias verticais do menu (`nav a::after`) em telas menores e adaptam os controles do carrossel ao toque.
* **Acessibilidade e Semântica:** Uso rigoroso de tags semânticas (`header`, `nav`, `main`, `section`, `article`, `figure`, `figcaption`, `blockquote`, `footer`), atributos ARIA (`aria-current="page"`, `aria-labelledby`, `aria-hidden`) e estados de foco visíveis (`:focus-visible`).
* **Favicon Vetorial Embutido:** Ícone SVG minimalista com o monograma **NI** em dourado e fundo escuro codificado diretamente em Base64 no `<head>` de todas as páginas.

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
│   ├── global.html
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

---

## Autor

Desenvolvido por **LuciferMS91** — [GitHub](https://github.com)
