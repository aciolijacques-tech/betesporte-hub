# 07 — Calendário

> **Contexto:** Calendário de eventos, agenda e datas do setor de marketing.
> **Leia quando:** A pergunta envolver calendário, eventos, datas, horários ou agenda.

---

## Descrição

O calendário é uma aba nativa do BETesporte Marketing Hub — não é um sistema separado. Exibe data e hora em tempo real e permite cadastrar eventos do setor.

---

## Funcionalidades

- **Relógio em tempo real** — hora, minuto e segundo atualizando ao vivo
- **Data por extenso** em português
- **Visão mensal** — grade completa do mês
- **Visão semanal** — grade por hora (07h às 21h)
- **Criar evento** — clicando em qualquer dia ou no botão "+ Evento"
- **Editar evento** — abrindo o detalhe e clicando em Editar
- **Excluir evento** — com confirmação
- **Próximos eventos** — painel lateral com os 5 próximos eventos futuros

---

## Categorias de evento

| Categoria | Cor | Uso típico |
|---|---|---|
| **Campanha** | Azul | Início, fim ou marcos de campanhas |
| **Briefing** | Roxo | Reuniões de briefing |
| **Reunião** | Verde | Reuniões gerais do setor |
| **Ativação** | Âmbar | Ações de ativação presencial ou digital |
| **Prazo** | Vermelho | Deadlines e entregas |
| **Outro** | Cinza | Eventos diversos |

---

## Campos de um evento

| Campo | Obrigatório |
|---|---|
| Título | Sim |
| Data | Sim |
| Categoria | Sim |
| Hora início | Não |
| Hora fim | Não |
| Descrição | Não |
| Responsável | Não |

---

## Persistência

Os eventos são salvos via **localStorage** no navegador quando o hub roda como arquivo HTML local. Os dados permanecem mesmo fechando e reabrindo o arquivo.

---

## Acesso

O calendário é acessível por **todos os níveis hierárquicos** — não há restrição de acesso por cargo.

---

**Contextos relacionados:** `05_CAMPANHAS.md`, `10_SISTEMA.md`
