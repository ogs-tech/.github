# OGS Tech — Hub de Documentação

[English](README.md) · **Português**

> **Tecnologia que leva o seu negócio além.** · *Future Ready.*

Este é o hub de documentação de toda a organização **OGS Tech** (Odenir Gomes Solutions).
Ele é organizado em torno do **guarda-chuva de marca** — como o negócio empacota, vende e opera.
A documentação detalhada de cada produto vive no seu repositório; este hub enquadra e aponta.

- **Marca em primeiro lugar:** os docs são agrupados por marca (Partners, Studio, Engine), não por pasta.
- **Aponte, não duplique:** os docs de produto (tutoriais, how-to, referência, arquitetura) vivem
  em cada repo. Este hub enquadra cada produto e aponta para eles — **não** os copia.
- **Hub, não silo:** o que vive aqui é genuinamente org-wide — o guarda-chuva de marca, a
  explicação entre marcas e uma página de enquadramento por produto.

---

## O guarda-chuva num relance

```
OGS Tech (Odenir Gomes Solutions)
│
├── OGS Partners ........... premium · sob medida · alta margem · useogs.com/partners
│     ├── Engenharia ....... Alephee
│     └── Suporte .......... Noordhen
│
├── OGS Studio ............. escalável · empacota & vende · useogs.com/studio
│     ├── Press ............ Open Source (devs · self-host) / Cloud (agências · gerenciado)
│     ├── Co. ............. Serviços de TI para PMEs brasileiras (done-for-you, opera o Press)
│     └── Royale IQ ........ nicho de influencers · pro bono
│
└── OGS Engine ............ a sala de máquinas · constrói a tecnologia
      ├── Press ........... core do CMS → vira o OGS Studio Press
      ├── Agent AI ........ core de IA   → vira o app Royale IQ
      └── Superset AI ..... ferramenta desktop interna (ajuda o time a usar o Claude)
```

Veja [Arquitetura de Marca](explanation/brand-architecture.md) para o quadro completo e
[Como se conecta](explanation/how-it-connects.md) para o fluxo entre as marcas.
Para a *identidade* de marca — missão, valores, logo, cor, tipografia — veja [Brand](brand/).

---

## Navegue por marca

### 🤝 [OGS Partners](partners/) — *premium, sob medida*
| Produto | O que é | Docs |
|---|---|---|
| [Alephee](partners/alephee/) | Plataforma de integração com marketplaces (parceiro de engenharia) | [docs do repo ↗](https://github.com/ogs-tech/alephee/tree/main/docs) |
| [Noordhen](partners/noordhen/) | Plataforma de operações personalizada da Noordhen Brasil (parceiro de suporte) | [docs do repo ↗](https://github.com/ogs-tech/noordhen/tree/main/docs) |

### 🏭 [OGS Studio](studio/) — *escalável, empacotado*
| Produto | O que é | Docs |
|---|---|---|
| [Press](studio/press/) | Plataforma de sites de conteúdo — três portas sobre um engine | [produto](studio/press/) |
| [Press Cloud](studio/press-cloud/) | Press SaaS gerenciado e multi-tenant (a porta Cloud) | [produto](studio/press-cloud/) |
| [Co.](studio/co/) | Serviços de TI done-for-you para PMEs | [produto](studio/co/) |
| [Royale IQ](studio/royale-iq/) | Coach com IA para jogadores de Clash Royale (pro bono) | [produto](studio/royale-iq/) |

### ⚙️ [OGS Engine](engine/) — *a sala de máquinas*
| Engine | O que é | Repo |
|---|---|---|
| [Press](engine/press/) | Core do CMS (scaffolder `@nis/create`) | [studio-press-cli ↗](https://github.com/ogs-tech/studio-press-cli) |
| [Agent AI](engine/agent-ai/) | Core de IA que move o Royale IQ | [royale-agent-ai-app ↗](https://github.com/ogs-tech/royale-agent-ai-app) |
| [Superset AI](engine/superset-ai/) | Apps desktop internos de tooling do Claude | [superset-ai-app ↗](https://github.com/ogs-tech/superset-ai-app) |

---

## Planejamento & quadros

O planejamento do dia a dia roda no **Trello**. Dois quadros espelham o guarda-chuva de marca:

| Quadro | Escopo |
|---|---|
| [OGS Tech HQ](https://trello.com/b/JpvCIoWc/ogs-tech-hq) | Toda a organização — marcas, GTM, operações |
| [OGS Tech Engine](https://trello.com/b/3lPid3OR/ogs-tech-engine) | A sala de máquinas — engenharia & execução de produto |

> O acesso é restrito ao time OGS. Esses quadros são a fonte da verdade do *trabalho em
> andamento*; este hub documenta o quadro *estável*.

---

## Convenções para quem contribui

- **Idioma:** inglês. (As versões `README.pt-BR.md` traduzem os hubs principais.)
- **Uma casa por codebase:** um repo é documentado uma vez sob sua marca principal. A Engine guarda
  o enquadramento *técnico*; o Studio guarda o de *produto / go-to-market* e faz cross-link.
- **Aponte, não duplique:** os docs detalhados vivem em cada repo — a página de produto aqui
  aponta para eles, não os copia.
- **Só Markdown:** sem build, sem dependências (veja [CLAUDE.md](../CLAUDE.md)).

---

*Odenir Gomes Solutions (OGS) · CNPJ 54.705.657/0001-83 · São Paulo/SP · fundada em 2024-04-12*
*[ogsolucoes.com.br](https://ogsolucoes.com.br)*
