# Plano de Criação do Site — Angatuba Motores | Loja & Oficina 🛠️⚡

Este documento estabelece o plano executivo, técnico e de design para o desenvolvimento da landing page de alta conversão da **Angatuba Motores**, com foco prioritário em dispositivos móveis (*Mobile-First*), identidade visual alinhada à loja física e direcionamento inteligente para o WhatsApp.

---

## 1. Dados Cadastrais & Informações do Negócio

As informações abaixo foram consolidadas com base no perfil do negócio e extraídas diretamente da imagem da fachada ([LojaFachada.jpg](./LojaFachada.jpg)):

* **Nome Comercial:** Angatuba Motores | Loja & Oficina
* **Atuação:** 
  * 🏪 **Loja:** Motores elétricos, bombas d'água, roçadeiras e materiais elétricos.
  * 🛠️ **Oficina:** Consertos, rebobinamento e instalações elétricas/mecânicas.
* **Endereço Físico (extraído da fachada):** Rua Major Pereira de Moraes, nº 858 – Angatuba – SP
* **WhatsApp de Contato:** `(15) 99614-5059` (Link internacional: `+5515996145059`)
* **Público-Alvo:** Moradores locais, produtores rurais, chacareiros, eletricistas, construtores e indústrias da região de Angatuba.

---

## 2. Identidade Visual & Design System

A paleta de cores e o sistema tipográfico foram extraídos diretamente da fachada da loja física, combinando o aspecto robusto da mecânica pesada com a precisão do setor elétrico.

### 2.1 Paleta de Cores Oficial

| Amostra | Nome da Cor | Hexadecimal | Papel / Aplicação |
| :--- | :--- | :--- | :--- |
| 🟦 | **Azul Industrial Escuro** | `#102A45` | Fundo do cabeçalho, rodapé e títulos institucionais. Transmite robustez e confiança técnica. |
| 🔷 | **Azul Aço / Céu** | `#87B8F3` | Tom secundário presente na sinalização, linhas de destaque e tags de categoria. |
| 🟨 | **Amarelo Elétrico** | `#F59E0B` | Cor de destaque (accent): ícones de raio/energia ⚡, badges de aviso e detalhes em botões secundários. |
| ⬛ | **Cinza Grafite / Slate** | `#1E293B` | Tipografia de títulos e cartões de serviços. |
| 🌫️ | **Cinza Neutro Suave** | `#64748B` | Textos secundários, legendas e descrições técnicas. |
| ⬜ | **Branco Puro / Gelo** | `#FFFFFF` / `#F8FAFC` | Fundo principal da página (assegura contraste máximo sob sol forte no celular). |
| 🟩 | **Verde Conversão** | `#25D366` | **Exclusivo para botões de CTA do WhatsApp** (máxima taxa de clique). |

### 2.2 Tipografia

* **Fonte de Títulos & Destaques (Display / Headings):**
  * Família: `Montserrat` ou `Inter` (Sans-Serif geométrica em pesos 700 e 800).
  * Justificativa: Letras maiúsculas, limpas e sólidas, fiéis à tipografia da placa de identificação da fachada (`MOTORES ELÉTRICOS`).
* **Fonte de Texto Corrido (Body):**
  * Família: `Inter` ou fontes nativas do sistema (`system-ui, -apple-system, sans-serif`).
  * Justificativa: Leitura confortável, altura de x alta e carregamento com zero latência no mobile.
* **Ícones:** Ícones SVG leves (temas de ferramentas, eletricidade, localização e telefone).

---

## 3. Arquitetura da Página (Mobile-First Wireframe)

A estrutura da página foi enxugada para manter foco total no que importa ao cliente: identificação imediata, portfólio de produtos/serviços e contato instantâneo.

```
┌────────────────────────────────────────────────────────┐
│ 1. HEADER FIXO (Logo + Horário + Botão Rápido Whats)   │
├────────────────────────────────────────────────────────┤
│ 2. HERO PRINCIPAL (Foto Fachada + Chamada + 2 CTAs)    │
│    [🛠️ Orçamento de Oficina]  [🔌 Peças da Loja]      │
├────────────────────────────────────────────────────────┤
│ 3. SEÇÃO LOJA (Produtos & Materiais Elétricos)         │
│    • Motores • Bombas • Roçadeiras • Elétrica          │
│    [Botão WhatsApp: Consultar Estoque]                 │
├────────────────────────────────────────────────────────┤
│ 4. SEÇÃO OFICINA (Serviços Especializados)             │
│    • Rebobinamento • Manutenção Bombas • Consertos     │
│    [Botão WhatsApp: Solicitar Orçamento]               │
├────────────────────────────────────────────────────────┤
│ 5. LOCALIZAÇÃO & HORÁRIOS                              │
│    • Rua Major Pereira de Moraes, 858 - Angatuba/SP    │
│    [Botão: Abrir no Google Maps / GPS]                 │
├────────────────────────────────────────────────────────┤
│ 6. RODAPÉ INSTITUCIONAL (Redes + Dados de Contato)     │
└────────────────────────────────────────────────────────┘
          [🟢 BOTÃO FLUTUANTE DO WHATSAPP FIXO]
```

### Detalhamento das 6 Seções

#### 1. Header Fixo (Sticky Header)
* **Logo:** Texto com design técnico `Angatuba Motores` + ícones `🛠️⚡`.
* **Badge de Status:** Ponto verde pulsante indicando disponibilidade.
* **Ação Imediata:** Botão compacto verde com ícone do WhatsApp para conversão rápida sem rolagem.

#### 2. Hero Principal (Primeira Dobra)
* **Visual:** Foto estilizada da fachada ([LojaFachada.jpg](./LojaFachada.jpg)) com sobreposição em gradiente escuro (`#102A45` translúcido) para contraste de leitura.
* **Título H1:** *"Sua Loja e Oficina Especializada em Motores, Bombas e Materiais Elétricos em Angatuba."*
* **Subtítulo:** *"Venda de peças, equipamentos e serviços autorizados de conserto e rebobinamento com agilidade e garantia."*
* **Botões Duplos de CTA:**
  * `🛠️ Orçamento de Oficina` (leva direto ao WhatsApp com texto pré-definido de serviço).
  * `🔌 Consultar Produtos da Loja` (leva ao WhatsApp com mensagem de cotação de peças).

#### 3. Seção Loja (Produtos & Materiais)
Cartões com ícones e visual moderno com os 4 grupos principais:
1. **Motores Elétricos:** Monofásicos, trifásicos, flangeados e de alta rotação.
2. **Bombas d'Água:** Bombas submersas (para poço artesiano), centrífugas, periféricas e injetoras.
3. **Roçadeiras & Motores a Combustão:** Ferramentas, lâminas, carretéis, carburadores e peças de reposição.
4. **Materiais Elétricos em Geral:** Fios, cabos, contatores, disjuntores, relés térmicos, capacitores e quadros de comando.
* **CTA Integrado:** Botão largo *"Consultar Preço ou Disponibilidade no WhatsApp"*.

#### 4. Seção Oficina & Serviços Técnicos
Apresentação em formato de lista interativa com cartões de serviços:
* **Rebobinamento de Motores:** Enrolamento de precisão com isolamento classe H e testes de bancada.
* **Manutenção de Bombas d'Água:** Troca de selos mecânicos, rolamentos, rotores e vedação completa.
* **Conserto de Roçadeiras e Ferramentas:** Regulagem de carburação, partida retrátil e revisão geral.
* **Painéis & Instalações Elétricas:** Montagem de quadros de partida e automação de bombas.
* **CTA Integrado:** Botão largo *"Trazer Equipamento para Avaliação"*.

#### 5. Localização, Rota & Horários
* **Endereço em destaque:** `Rua Major Pereira de Moraes, nº 858 – Angatuba – SP`.
* **Botão de Rota 1-Click:** `"Abrir no Google Maps / GPS"` (abre diretamente o app de navegação do celular do cliente).
* **Quadro de Horários:**
  * Segunda a Sexta: 07h30 às 18h00.
  * Sábado: 07h30 às 12h00.
* **Telefone Fixo / WhatsApp:** `(15) 99614-5059`.

#### 6. Rodapé & Botão Flutuante de Alta Conversão
* Botão flutuante do WhatsApp no canto inferior direito (`position: fixed; bottom: 20px; right: 20px; z-index: 50`), com efeito de pulso suave.
* Copyright, informações de Angatuba/SP e link direto para o Instagram `@angatuba_motores`.

---

## 4. Estratégia de Roteamento de Mensagens do WhatsApp

Cada botão do site terá uma URL parametrizada (`https://wa.me/5515996145059?text=...`) para que a equipe receba o cliente já sabendo exatamente qual é a demanda:

| Ponto de Origem | Mensagem Pré-configurada no Link |
| :--- | :--- |
| **Header / Botão Geral** | `Olá! Vi o site da Angatuba Motores e gostaria de tirar uma dúvida.` |
| **Hero (Oficina)** | `Olá! Gostaria de um orçamento para conserto/manutenção de equipamento.` |
| **Hero (Loja)** | `Olá! Gostaria de consultar o preço e estoque de um produto/material elétrico.` |
| **Card Motores / Bombas** | `Olá! Preciso de informações sobre motores e bombas disponíveis.` |
| **Card Materiais Elétricos** | `Olá! Gostaria de uma cotação de materiais elétricos (fios, disjuntores, peças).` |
| **Botão Flutuante** | `Olá! Estou no site da Angatuba Motores e preciso de atendimento.` |

---

## 5. Especificações Técnicas de Implementação

* **Stack Recomendada:** HTML5 Semântico + Tailwind CSS + Vanilla JS para interatividades leves (carregamento instantâneo).
* **Performance:**
  * Imagem de fundo responsiva e otimizada (`LojaFachada.jpg`).
  * Tempo de carregamento estimado: **< 0.8s** em rede móvel 4G.
* **SEO Local & Rich Snippets (Schema.org):**
  * Inclusão do metadado JSON-LD `LocalBusiness` / `AutoRepair` para indexação imediata no Google de Angatuba e região.
* **Metatags Open Graph:** Configuração de imagem, título e descrição para que ao compartilhar o link no WhatsApp, apareça um preview profissional com a foto da fachada.

---

## 6. Próximos Passos para Execução

1. **Aprovação deste plano.**
2. **Criação do código-fonte:** Geração do `index.html` com layout mobile-first estilizado com Tailwind CSS.
3. **Integração dos assets:** Aplicação da foto da fachada com corte otimizado e testes dos links de WhatsApp.
4. **Deploy de teste:** Configuração para publicação instantânea.
