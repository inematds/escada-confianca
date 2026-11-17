# 🪜 Escada da confiança

🎬 Vídeo: https://www.youtube.com/watch?v=V-7fJ1SjlpQ

[![Escada da confiança — seu agente só diz pronto depois de provar](guia/assets/banner.jpg)](https://inematds.github.io/escada-confianca/guia/)

**🇧🇷 [Português](README.md) · 🇺🇸 [English](README.en.md) · 🇪🇸 [Español](README.es.md)**

Você pede uma coisa para a IA, ela diz pronto, e você perde a tarde conferindo. Uma engenheira da SpaceX acordou com 20 entregas prontas dos agentes dela. Com a **escada da confiança**, o seu agente só diz pronto depois de provar.

## O que é

Quando a IA diz “pronto” sem ter testado, quem confere é você, e isso come a tarde. A **escada da confiança** é um método em três degraus para o seu agente de programação (Claude Code ou Codex) só entregar com prova: ele usa o que fez como um usuário e mostra um recibo, passa numa avaliação com nota 10 de 10 e transforma cada erro repetido numa regra que o computador cobra sozinho. É para quem já usa agentes de IA no código e quer conferir menos. O kit traz textos prontos para colar no seu projeto e um exemplo que roda só com Python.

## 📖 Guia de uso

Guia completo (landing + passo a passo): **https://inematds.github.io/escada-confianca/guia/**

## O kit

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

Requer Python 3.9 ou mais novo, sem bibliotecas extras.

## Créditos

O método é da **Lauren Tan** (@poteto), engenheira de software na SpaceXAI (time do Grok Bot), antes no Cursor.

- **Entrevista original** — workshop ao vivo na Maven, "How Cursor Turned AI Agents Into Better Engineers" (12/08/2026): https://maven.com/p/e23d9c/how-cursor-turned-ai-agents-into-better-engineers
- **Cópia do workshop no YouTube** (não oficial, postada por terceiros): https://www.youtube.com/watch?v=Cmoh-yR-usA
- **pstack**, o pacote de habilidades dela: https://github.com/cursor/plugins/tree/main/pstack
- Palestra "All Code Is Slop (Except Mine)" (AI Engineer): https://www.youtube.com/watch?v=O_zcc6Xl12g
- Perfil: https://x.com/poteto

Detalhes em [CREDITOS.md](CREDITOS.md). Licença MIT. Feito pelo [INEMA.CLUB](https://inema.club).
