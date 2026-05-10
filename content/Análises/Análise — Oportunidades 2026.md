---
tipo: analise
candidata: Dra. Cristiany
referencia: eleicoes-2022
tags: [analise, estrategia, 2026]
---

# 📈 Análise — Oportunidades para 2026

## Resumo Executivo
Em 2022, a Dra. Cristiany obteve **33,198 votos** em **645 municípios** do Estado de São Paulo.
A análise dos dados revela oportunidades claras de crescimento para 2026.

## 🔴 Prioridade 1 — 100 municípios com ZERO votos
Esses municípios não tiveram nenhum voto registrado em 2022.
São **territórios virgens** com alto potencial de crescimento.

```dataview
TABLE cidade AS "Município"
FROM "Candidatos/Dra. Cristiany/Cidades 2022"
WHERE votos = 0
SORT cidade ASC
```

## 🟡 Prioridade 2 — Municípios com 1 a 50 votos
Presença mínima — potencial de triplicar ou quadruplicar com trabalho de base.

```dataview
TABLE cidade AS "Município", votos AS "Votos"
FROM "Candidatos/Dra. Cristiany/Cidades 2022"
WHERE votos > 0 AND votos <= 50
SORT votos ASC
```

## ⭐ Base forte — Municípios acima de 500 votos
Esses municípios são a base eleitoral consolidada. Foco em manter e ampliar.

```dataview
TABLE cidade AS "Município", votos AS "Votos", ranking AS "Rank"
FROM "Candidatos/Dra. Cristiany/Cidades 2022"
WHERE votos > 500
SORT votos DESC
```

## 🗺 Links
- [[Eleições 2022 — Painel Geral]]
- [[Dra. Cristiany — Perfil]]
