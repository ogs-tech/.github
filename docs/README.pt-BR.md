# OGS Tech — Hub de Documentação

[English](README.md) · **Português**

> **Tecnologia que leva o seu negócio além.** · *Future Ready.*

Este é o hub de documentação de toda a organização **OGS Tech** (Odenir Gomes Solutions).
Ele é organizado em torno do **guarda-chuva de marca** — como o negócio empacota, vende e
opera — e segue o framework [Diátaxis](https://diataxis.fr) dentro de cada produto.

- **Marca em primeiro lugar:** os docs são agrupados por marca (Partners, Studio, Engine), não por pasta.
- **Diátaxis por dentro:** todo produto tem *Tutoriais*, *Guias how-to*, *Referência* e *Explicação*.
- **Hub, não silo:** este hub guarda a visão guarda-chuva e a referência por produto. Docs profundos,
  próximos ao código, continuam vivendo em cada repositório — o hub **aponta** para eles.

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
| [Alephee](partners/alephee/) | Plataforma de integração com marketplaces (parceiro de engenharia) | [referência](partners/alephee/reference/) |
| [Noordhen](partners/noordhen/) | Plataforma de operações personalizada da Noordhen Brasil (parceiro de suporte) | [referência](partners/noordhen/reference/) |

### 🏭 [OGS Studio](studio/) — *escalável, empacotado*
| Produto | O que é | Docs |
|---|---|---|
| [Press](studio/press/) | Plataforma de sites de conteúdo — OSS (self-host) e Cloud (agências) | [referência](studio/press/reference/) |
| [Co.](studio/co/) | Serviços de TI done-for-you para PMEs | [explicação](studio/co/explanation/) |
| [Royale IQ](studio/royale-iq/) | Coach com IA para jogadores de Clash Royale (pro bono) | [referência](studio/royale-iq/reference/) |

### ⚙️ [OGS Engine](engine/) — *a sala de máquinas*
| Engine | O que é | Docs |
|---|---|---|
| [Press](engine/press/) | Core do CMS (scaffolder `@nis/create`) | [referência](engine/press/reference/) |
| [Agent AI](engine/agent-ai/) | Core de IA que move o Royale IQ | [referência](engine/agent-ai/reference/) |
| [Superset AI](engine/superset-ai/) | Apps desktop internos de tooling do Claude | [referência](engine/superset-ai/reference/) |

---

## Entendendo o framework

Cada pasta de produto usa os quatro quadrantes Diátaxis:

| Quadrante | Orientação | Responde |
|---|---|---|
| 📚 **Tutoriais** | aprendizado | "Me ensine, passo a passo" |
| 🔧 **Guias how-to** | tarefas | "Como faço X?" |
| 📖 **Referência** | informação | "Qual é a API / comando / config exata?" |
| 💡 **Explicação** | compreensão | "Por que foi construído assim?" |

> Nesta primeira leva, **Referência** e **Explicação** são escritas a partir dos repositórios
> reais; **Tutoriais** e **How-to** são stubs guiados, prontos para preencher.

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
  a referência *técnica*; o Studio guarda o enquadramento de *produto / go-to-market* e faz cross-link.
- **Aponte, não duplique:** se um repo já tem boa documentação, aponte para ela a partir de `reference/`.
- **Só Markdown:** sem build, sem dependências (veja [CLAUDE.md](../CLAUDE.md)).

---

*Odenir Gomes Solutions (OGS) · CNPJ 54.705.657/0001-83 · São Paulo/SP · fundada em 2024-04-12*
*[ogsolucoes.com.br](https://ogsolucoes.com.br)*
