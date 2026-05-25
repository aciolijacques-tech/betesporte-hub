# 09 — Relatórios

> **Contexto:** Geração e exportação de relatórios executivos.
> **Leia quando:** A pergunta envolver relatórios, exportação, prévia ou apresentação para liderança.

---

## Descrição

O módulo de relatórios gera documentos prontos para apresentar à liderança, com base nos dados cadastrados no hub. Funciona em 3 passos.

---

## Tipos de relatório disponíveis

| Tipo | Público-alvo | Conteúdo |
|---|---|---|
| **Executivo** | CMO / Diretoria | KPIs principais, destaques, status geral |
| **Completo** | Gerência | Toda a carteira, campanhas, produtos e rankings |
| **Carteira** | Interno | Perfis, plataformas, engajamento e vínculos |
| **Campanhas** | Gerência | Campanhas, produtos vinculados, verbas e status |

---

## Seções configuráveis por tipo

### Tipo: Executivo
- Cabeçalho (data, cargo, marca)
- KPIs principais
- Status do ecossistema
- Destaques da carteira (top 3)
- Resumo de campanhas

### Tipo: Completo
- Cabeçalho
- KPIs
- Status
- Carteira completa de influenciadores
- Campanhas detalhadas
- Catálogo de produtos
- Rankings de performance

### Tipo: Carteira
- Cabeçalho
- KPIs da carteira
- Distribuição por porte e plataforma
- Carteira completa
- Rankings

### Tipo: Campanhas
- Cabeçalho
- Campanhas detalhadas
- Mapa de vínculos

---

## Fluxo de geração

1. **Escolher tipo** de relatório
2. **Selecionar seções** a incluir (cada seção pode ser ligada/desligada)
3. **Prévia + Exportar** — visualizar antes de baixar

---

## Formatos de exportação

| Formato | Ação |
|---|---|
| **Baixar HTML** | Gera arquivo `.html` para abrir no navegador ou imprimir como PDF |
| **Copiar texto** | Copia o conteúdo para colar em Word, e-mail ou apresentação |

---

## Restrições de conteúdo

- Dados financeiros (cachê, verba) só aparecem no relatório se o usuário for **nível 3 ou acima**
- O relatório respeita o perfil ativo no momento da geração

---

## Formato do cabeçalho

```
═══════════════════════════════════════════
  BETesporte — TIPO DO RELATÓRIO
  Gerado em: DD de Mês de AAAA
  Gerado por: [Cargo do usuário]
═══════════════════════════════════════════
```

---

**Contextos relacionados:** `08_METRICAS.md`, `02_HIERARQUIA.md`
