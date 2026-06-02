# Noordhen

> Custom operations platform — the **Support** partner under [OGS Partners](../).

A bespoke digital platform and service ecosystem for **Noordhen Brasil** (a 25+ year hygiene
products supplier). It supports operations, scheduling, documents, and team communication, across
two parallel environments: **Production** and **CProd** (a secondary instance).

- **Brand:** OGS Partners · Support
- **Repository:** [`ogs-tech/noordhen`](https://github.com/ogs-tech/noordhen) · folder `noordhen/`
- **Authoritative docs:** [`noordhen/docs/`](https://github.com/ogs-tech/noordhen/tree/main/docs) — the repo's own Diátaxis portal. This hub frames Noordhen in the OGS umbrella; the portal is the working source.

## Documentation (Diátaxis)

| | |
|---|---|
| 📚 [Tutorials](tutorials/) | Learn the platform step by step |
| 🔧 [How-to guides](how-to/) | Run a backup, deploy an environment… |
| 📖 [Reference](reference/) | Sub-projects, stacks, commands, environments |
| 💡 [Explanation](explanation/) | Why the Production/CProd split exists |

## At a glance

| Sub-project | Purpose | Stack |
|---|---|---|
| **noordhen-react-app** | Production front-end | React 16 · Bootstrap 4 · Styled Components · Syncfusion Schedule |
| **noordhen-backup-nest-api** | Backup automation service | NestJS 10 · Prisma 6 · MySQL · node-ssh |

External repos (not in this folder): `noordhen-strapi-api`, `noordhen-cprod-react-app`,
`noordhen-cprod-strapi-api`.
