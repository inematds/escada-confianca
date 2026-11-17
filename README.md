# 🪜 Escada da confiança

Seu agente de IA diz "pronto" e você perde a tarde conferindo. A **escada da confiança** faz o agente provar o que fez, ganhar nota e transformar cada erro em regra — o método da engenheira Lauren Tan (SpaceXAI / Grok Bot, ex-Cursor), em kit para Claude Code e Codex.

- `kit/degrau1-prova/` — skill "provar antes de dizer pronto" + mapa de telas
- `kit/degrau2-nota/` — avaliação com nota e prompt do juiz (outro modelo)
- `kit/degrau3-regra/` — o erro vira regra + registro de erros
- `kit/AGENTS-escada.md` — bloco para colar no CLAUDE.md / AGENTS.md
- `exemplo/escada.py` — os 3 degraus num exemplo que roda só com Python

```bash
python3 exemplo/escada.py cadastro_quebrado    # 0/3 degraus
python3 exemplo/escada.py cadastro_corrigido   # 3/3: PRONTO com prova
python3 -m unittest discover -s tests -v
```

Créditos e link da entrevista original: [CREDITOS.md](CREDITOS.md).
