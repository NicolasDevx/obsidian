---
candidata: 
eleicao: 
total_municipios: 
total_votos: 
tags: [painel, eleicao]
---

# {{candidata}} — Eleições {{eleicao}}

## 🔢 Números Gerais
| Indicador | Valor |
|---|---|
| Total de municípios | |
| Total de votos | |
| Zero votos | |
| Acima de 200 votos | |

## 🏆 Top 30%
```dataview
TABLE cidade, votos
FROM "Candidatos/{{candidata}}/Cidades {{eleicao}}"
SORT votos DESC
LIMIT 194
```

## 🔴 Zero Votos
```dataview
TABLE cidade
FROM "Candidatos/{{candidata}}/Cidades {{eleicao}}"
WHERE votos = 0
SORT cidade ASC
```
