# Angatuba Motores

Página institucional e comercial para a loja e oficina **Angatuba Motores** (Angatuba - SP), voltada à apresentação de produtos, serviços técnicos e direcionamento de clientes para atendimento via WhatsApp.

## Estrutura do Projeto

```text
.
├── index.html        # Página única (HTML5 + Tailwind CSS via CDN)
├── Logo.jpg          # Logotipo da empresa e favicon
├── LojaFachada.jpg   # Fotografia da fachada física
└── README.md         # Documentação do repositório
```

## Seções da Página

1. **Header Fixo:** Identificação da marca, links de navegação rápida e botão direto para o WhatsApp.
2. **Hero:** Apresentação principal da loja e oficina, fotografia da fachada e atalhos para orçamento de oficina ou consulta de peças.
3. **Loja e Serviços de Oficina:**
   - **Produtos e Materiais Elétricos:** Motores elétricos, bombas d'água, roçadeiras, peças de reposição e materiais elétricos.
   - **Serviços de Oficina:** Rebobinamento de motores, manutenção de bombas, conserto de roçadeiras (2T/4T) e montagem de quadros de comando.
4. **Localização e Horários:** Endereço físico, horários de funcionamento, telefone para ligação direta e mapa interativo do Google Maps.
5. **Rodapé e Botão Flutuante:** Links institucionais, Instagram e botão fixo para contato via WhatsApp.

## Especificações Técnicas

- **Marcação:** HTML5 semântico com dados estruturados JSON-LD (`Schema.org/LocalBusiness`) e metatags Open Graph.
- **Estilização:** Tailwind CSS (configurado com paleta baseada na identidade visual da fachada e logotipo).
- **Tipografia:** `Montserrat` (títulos) e `Inter` (textos), carregadas via Google Fonts.
- **Paleta de Cores:**
  - `#050B14` / `#0A1628` — Azul marinho escuro (Header, Hero, Oficina e Rodapé)
  - `#0F172A` — Grafite escuro (Seção de Localização)
  - `#1D4ED8` / `#60A5FA` — Azul royal e azul claro (Destaques e botões institucionais)
  - `#F1F5F9` / `#FFFFFF` — Superfícies claras e cartões da loja
  - `#25D366` — Verde (Botões de ação para o WhatsApp)

## Informações da Empresa

- **Endereço:** Rua Major Pereira de Moraes, nº 858, Angatuba – SP, CEP 18240-000
- **Telefone / WhatsApp:** (15) 99614-5059
- **Horário de Funcionamento:** Segunda a Sexta das 07h30 às 18h00 | Sábado das 07h30 às 12h00

## Execução Local

Como o projeto é estático e não possui dependências de build, basta abrir o arquivo `index.html` diretamente no navegador ou servir o diretório localmente:

```bash
python3 -m http.server 8080
```

Acesse em `http://localhost:8080`.
