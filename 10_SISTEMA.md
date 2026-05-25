# 10 — Configuração Técnica do Sistema

> **Contexto:** Como o hub funciona tecnicamente — stack, persistência, estrutura de abas.
> **Leia quando:** A pergunta envolver como o sistema funciona, dados salvos, tecnologia ou estrutura do hub.

---

## Stack tecnológica

| Componente | Tecnologia |
|---|---|
| Interface | HTML + CSS + JavaScript puro (sem frameworks) |
| Estilo | CSS customizado com variáveis (design system próprio) |
| Ícones | Tabler Icons (CDN) |
| Fontes | Syne (display) + DM Sans (corpo) via Google Fonts |
| Armazenamento | localStorage do navegador (standalone) |
| Armazenamento (Claude) | window.storage API do Claude Artifacts |

---

## Estrutura de abas (navegação)

| Aba | ID | Descrição |
|---|---|---|
| Visão geral | `visao` | Dashboard com KPIs e status |
| Calendário | `calendario` | Agenda com relógio em tempo real |
| Métricas | `metricas` | Gráficos e rankings |
| Relatório | `relatorio` | Gerador de relatórios |
| Comunicação | `comunicacao` | Mensagens internas |
| Hierarquia | `hierarquia` | Estrutura do time |
| Influenciadores | `influenciadores` | Carteira completa |
| Produtos | `produtos` | Catálogo |
| Campanhas | `campanhas` | Gestão de campanhas |

---

## Chaves de armazenamento (localStorage)

| Chave | Conteúdo |
|---|---|
| `betesporte_influenciadores` | Array de influenciadores |
| `betesporte_produtos` | Array de produtos |
| `betesporte_campanhas` | Array de campanhas |
| `betesporte_mensagens` | Array de mensagens |
| `betesporte_lidas` | Set de IDs de mensagens lidas |
| `betesporte_calendario_eventos` | Array de eventos do calendário |

---

## Hierarquia de perfis no sistema

O hub usa um seletor "Visualizando como" que simula o nível de acesso. Em produção real, isso seria substituído por autenticação real (Google OAuth ou similar).

Valores: `cmo`, `diretor`, `gerente`, `coordenador`, `social_media`, `video_maker`, `designer`

---

## Persistência de dados

- **No Claude (artifacts):** via `window.storage` — persiste entre sessões da mesma conversa
- **No arquivo HTML baixado:** via `localStorage` — persiste no navegador do usuário
- **Sem backend:** todos os dados ficam no cliente

---

## Limitações atuais

| Limitação | Impacto |
|---|---|
| Sem autenticação real | Qualquer pessoa pode mudar o perfil manualmente |
| Sem backend | Dados não são compartilhados entre dispositivos |
| Sem Google OAuth | Login social não funciona no ambiente atual |
| Sem banco de dados | Dados perdidos se o usuário limpar o localStorage |

---

## Próximas evoluções possíveis

1. **Login com Google OAuth** — exige hospedagem em servidor (Netlify, Vercel)
2. **Firebase** — banco de dados em nuvem + autenticação Google nativa
3. **Cowork / Claude** — uso via automação com os arquivos MD como base de contexto

---

## Paleta de cores do design

| Variável | Valor | Uso |
|---|---|---|
| `--accent` | `#2563EB` | Azul principal |
| `--accent2` | `#60A5FA` | Azul claro / destaques |
| `--green` | `#4ADE80` | Status positivos |
| `--amber` | `#FBBF24` | Alertas / em andamento |
| `--red` | `#F87171` | Erros / urgente |
| `--bg` | `#0A0A0F` | Fundo principal |
| `--text` | `#EDF2FF` | Texto principal |

---

**Contextos relacionados:** `01_PROJETO.md`
