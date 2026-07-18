# Sobre a OGS tech

[English](README.md) · **Português**

## Missão

Tecnologia que leva o seu negócio além.

---

## Propósito

Tecnologia de qualidade não deveria ser privilégio de empresa grande.

---

## Visão

Ser a maior empresa de tecnologia pra pequenas e médias empresas do Brasil.

---

## Valores

Lideramos com ética, crescemos com pessoas.

---

## Slogan

Your business. Further. Future-Ready.

> Redação canônica: [Brand → Company](../../docs/brand/company.md) — mantenha as duas em sincronia.

---

## Guarda-chuva de Marca

A OGS tech opera como um **guarda-chuva de marca**: três marcas, uma tecnologia por baixo, cada uma
uma forma diferente de ir ao mercado.

| Marca | Papel | Vai ao mercado como |
|---|---|---|
| 🤝 **OGS Partners** | *premium, sob medida* | Serviços de Engenharia e Suporte para empresas parceiras (Alephee, Noordhen) |
| 🏭 **OGS Studio** | *produtos escaláveis* | Produtos empacotados, vendidos em escala (o Press, o Royale IQ) |
| ⚙️ **OGS Engine** | *a sala de máquinas* | Constrói a tecnologia e executa os projetos da Partners (Press, Agent AI, Superset AI) |

➡️ Quadro completo: [Arquitetura de Marca — o guarda-chuva OGS](https://github.com/ogs-tech/.github/blob/main/docs/explanation/brand-architecture.md)

---

## Organograma

O organograma abaixo segue boas práticas comuns: hierarquia clara de cima para baixo, responsabilidades agrupadas por área e uma descrição curta dentro de cada cartão de papel. No estágio atual da OGS tech, **Odenir Gomes** lidera as áreas de Liderança, Tecnologia e Produto, enquanto **Rosana Pinto** lidera as áreas Comercial e de Operações — com **Marketing** liderado por **Synue Cunioci**.

```mermaid
%%{init: {"flowchart": {"nodeSpacing": 55, "rankSpacing": 95, "diagramPadding": 28, "useMaxWidth": true}}}%%
flowchart TB

    CEO["Odenir Gomes<br/>Fundador & CEO<br/>Estratégia, produto, entrega e crescimento"]

    CEO --> TECH["Head de Tecnologia<br/>Arquitetura, engenharia e plataforma<br/>Odenir Gomes"]
    CEO --> PRODUCT["Head de Produto<br/>Roadmap, discovery e priorização<br/>Synue Cunioci"]
    CEO --> BUSINESS["Head Comercial<br/>Vendas, parcerias e posicionamento<br/>Rosana Pinto"]
    CEO --> OPS["Head de Operações<br/>Fluxo de entrega, atendimento e continuidade<br/>Rosana Pinto"]

    TECH --> SDE["Desenvolvimento de Software<br/>Entrega de features e qualidade de código<br/>Odenir Gomes"]
    TECH --> DEVOPS["DevOps / Infraestrutura<br/>Cloud, deploy e confiabilidade<br/>Odenir Gomes"]

    PRODUCT --> PM["Gestão de Produto<br/>Requisitos, validação e planejamento<br/>Synue Cunioci"]
    PRODUCT --> DESIGN["Design / UX<br/>Usabilidade, interfaces e consistência<br/>Synue Cunioci"]

    BUSINESS --> SALES["Vendas<br/>Prospecção, propostas e fechamento<br/>Rosana Pinto"]
    BUSINESS --> MKT["Marketing<br/>Conteúdo, branding e presença digital<br/>Synue Cunioci"]

    OPS --> CS["Customer Success<br/>Onboarding, adoção e retenção<br/>Rosana Pinto"]
    OPS --> SUPPORT["Suporte<br/>Chamados, triagem e continuidade do serviço<br/>Rosana Pinto"]
    OPS --> FIN["Financeiro & Administrativo<br/>Fluxo de caixa, documentos e compliance<br/>Rosana Pinto"]

    classDef founder fill:#14133A,color:#F6F2ED,stroke:#E39C19,stroke-width:2px;
    classDef heads fill:#DBDFFE,color:#14133A,stroke:#7C81F0,stroke-width:1.5px;
    classDef tech fill:#E5E0DB,color:#2B2722,stroke:#948E88,stroke-width:1.5px;
    classDef product fill:#F0F2FE,color:#201F53,stroke:#9CA4F9,stroke-width:1.5px;
    classDef growth fill:#FCDCB1,color:#704A02,stroke:#BF8107,stroke-width:1.5px;
    classDef ops fill:#CDC8C3,color:#1C1915,stroke:#756F68,stroke-width:1.5px;

    class CEO founder;
    class TECH,PRODUCT,BUSINESS,OPS heads;
    class SDE,DEVOPS tech;
    class PM,DESIGN product;
    class SALES,MKT growth;
    class CS,SUPPORT,FIN ops;
```

## Papéis e Responsabilidades Atuais

> No estágio atual da OGS tech, os papéis de Liderança, Tecnologia e Produto são ocupados por **Odenir Gomes**, enquanto os papéis Comercial e de Operações são ocupados por **Rosana Pinto** — exceto **Marketing**, liderado por **Synue Cunioci**.

| Área | Papel | Descrição | Colaborador atual |
|---|---|---|---|
| Liderança | Fundador / CEO | Define a direção da empresa e conecta estratégia com execução. | Odenir Gomes |
| Tecnologia | Head de Tecnologia | Cuida de arquitetura, qualidade de engenharia, infraestrutura e decisões técnicas. | Odenir Gomes |
| Tecnologia | Desenvolvimento de Software | Constrói e mantém os produtos e serviços core da empresa. | Odenir Gomes |
| Tecnologia | DevOps / Infraestrutura | Cuida do setup de cloud, do fluxo de deploy e da confiabilidade operacional. | Odenir Gomes |
| Produto | Head de Produto | Define as prioridades do roadmap e alinha a entrega às necessidades do cliente. | Synue Cunioci |
| Produto | Gestão de Produto | Organiza requisitos, validação e prioridades de execução. | Synue Cunioci |
| Produto | Design / UX | Melhora usabilidade, interfaces e consistência visual. | Synue Cunioci |
| Comercial | Head Comercial | Lidera parcerias, propostas e esforços de geração de receita. | Rosana Pinto |
| Comercial | Vendas | Qualifica oportunidades, conduz conversas e fecha negócios. | Rosana Pinto |
| Comercial | Marketing | Fortalece o posicionamento por meio de conteúdo e presença digital. | Synue Cunioci |
| Operações | Head de Operações | Coordena o fluxo de entrega, as rotinas internas e a continuidade do serviço. | Rosana Pinto |
| Operações | Customer Success | Apoia onboarding, adoção e valor de longo prazo para o cliente. | Rosana Pinto |
| Operações | Suporte | Recebe solicitações, faz triagem de problemas e coordena respostas. | Rosana Pinto |
| Operações | Financeiro e Administrativo | Organiza rotinas financeiras e administrativas e apoia o compliance. | Rosana Pinto |
