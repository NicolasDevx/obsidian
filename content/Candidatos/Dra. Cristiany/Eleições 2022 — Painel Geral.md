---
tipo: painel
candidata: Dra. Cristiany
eleicao: 2022
total_municipios: 645
total_votos: 33198
tags: [painel, eleicoes-2022, analise]
---

# 📊 Eleições 2022 — Painel Geral
> **Candidata:** Dra. Cristiany | **Estado:** São Paulo | **Ano:** 2022

## 🔢 Números Gerais
| Indicador | Valor |
|---|---|
| Total de municípios | 645 |
| Total de votos | 33,198 |
| Municípios com **zero votos** | 100 |
| Municípios acima de 200 votos | 31 |
| Top 10% (mais votados) | 65 cidades |
| Top 30% (mais votados) | 194 cidades |

---

## 🏆 Top 10% — Cidades mais votadas (65 municípios)
```dataview
TABLE cidade AS "Município", votos AS "Votos", faixa AS "Faixa"
FROM "Candidatos/Dra. Cristiany/Cidades 2022"
SORT votos DESC
LIMIT 65
```

---

## 📋 Top 30% — Cidades mais votadas (194 municípios)
```dataview
TABLE cidade AS "Município", votos AS "Votos", ranking AS "Rank"
FROM "Candidatos/Dra. Cristiany/Cidades 2022"
SORT votos DESC
LIMIT 194
```

---

## 🔴 Cidades com ZERO votos — Prioridade para 2026 (100 municípios)
```dataview
TABLE cidade AS "Município", faixa AS "Status"
FROM "Candidatos/Dra. Cristiany/Cidades 2022"
WHERE votos = 0
SORT cidade ASC
```

---

## 🟢 Cidades acima de 200 votos — Base forte (31 municípios)
```dataview
TABLE cidade AS "Município", votos AS "Votos"
FROM "Candidatos/Dra. Cristiany/Cidades 2022"
WHERE votos > 200
SORT votos DESC
```

---

## 📂 Links rápidos
- [[Dra. Cristiany — Perfil]]
- [[Análise — Oportunidades 2026]]
- [[AuraCamp — Sobre o Sistema]]
