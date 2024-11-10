# :pig: Finance.Ai

### Links of the project

- [Figma](<https://www.figma.com/design/ndIZ9nevfZZCMxCL4lZxfQ/FSW-Finance-(LIVE)?node-id=57-1074>)

- [Repository](https://github.com/felipemotarocha/fullstackweek-financeai)

##### Framework | SubLanguage

- [Next 14.2.16](https://nextjs.org)
- [Typescript](https://www.typescriptlang.org)

##### CSS

- [TailwindCSS](https://tailwindcss.com)
- [Plugin class sorting Prettier](https://tailwindcss.com/blog/automatic-class-sorting-with-prettier)
- Need Configuration file and extension

##### Correction code

- [ESlint](https://eslint.org)
- Need Extension

##### Services

- [PRISMA ORM](https://www.prisma.io)
- [SHADCN COMPONENTS](https://ui.shadcn.com/docs/installation/next)
- [CLERK - authenticatation]()

##### Database

- [NeonDB Host - private](https://console.neon.tech/app/projects)
- [PostgreSQL](https://www.prisma.io/postgres)

##### Libraries

- [ClerkThemes](https://clerk.com/docs/customization/themes)
- [HUSKY - Desenvolvimento](https://www.npmjs.com/package/husky)
- [LINT/STAGED - Desenvolvimento]()

##### Commits methods

- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)

### Initial Configs

- No for src/directory and no for alias @/ when i created the next projet
- Install prisma and init it: npm install prisma | npx prisma init
- Create database inside schema.prisma

### How to configure Husky, lint staged and commit-msg

- npm i -D git-commit-msg-linter
- npm i -D lint-staged
- npm i -D husky

##### :mag_right: Objetivos

- O lint-staged é usado para somente executar comandos em arquivos que estão preparados para o commit. Isso evita que o prettier ou qualquer biblioteca de organização rode em todos os arquivos ao mesmo tempo.

- O código para colar, é usado para procurar arquivos de extensão .ts ou .tsx e rodar o prettier.

- o git-commit-msg-linter força a inserção correta do conventional commits ao realizer um commit.

- Além disso, você precisa conectar o Husky ao git-commit-msg (conventional commits) para que os dois trabalhem juntos.

  1 - npx husky init
  2 - in the root of the project, create a file with the filename .lintstagedrc.json
  3 - then, paste it : { "\*.ts?(x)": ["eslint --fix", "prettier --write"] } without the first \.
  4 - create a file inside .husky commit-msg and put the code .git/hooks/commit-msg $1 inside it
  5 -
