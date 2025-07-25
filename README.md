# Comandos

npx prisma migrate dev

# App

GymPass Style App

## Requisitos funcionais

- [ ] Deve ser possível se cadastrar;
- [ ] Deve ser possível se autenticar;
- [ ] Deve ser possível obter o perfil de um usuário logado;
- [ ] Deve ser possível obter o número de check-ins realizados pelo usuário logado;
- [ ] Deve ser possível o usuário obter seu histórico de check-ins;
- [ ] Deve ser possível o usuário buscar academias próximas;
- [ ] Deve ser possível o usuário buscar academias pelo nome;
- [ ] Deve ser possível o usuário realizar check-in em uma academia;
- [ ] Deve ser possível validar o check-in de um usuário;
- [ ] Deve ser possível cadastrar uma academia;

## Regras de negócio

- [ ] O usuário não deve poder se cadastrar com um email duplicado;
- [ ] O usuário não pode fazer 2 check-ins no mesmo dia;
- [ ] O usuário não pode fazer check-in se não estiver perto (100 mt) da academia;
- [ ] O check-in só pode ser validado até 20 minutos após criado;
- [ ] O check-in só pode ser validado por administradores;
- [ ] a academia só pode ser cadastrada por administradores;

## Requisitos não funcionais

- [ ] A senha do usuário precisa estar criptografada;
- [ ] Os dados da aplicação precisam estar persistidos em um banco PostgreSQL;
- [ ] Todas as listas de dados precisam estar paginadas com 20 itens por página;
- [ ] O usuário deve ser identificado por um JWT (JSON Web Token);

## Setup

npm init -y
npm i typescript @types/node tsx tsup -D
npx tsc --init
npm i fastify
npm i dotenv
npm i zod
npm i eslint @rocketseat/eslint-config -D
npm i prisma -D
npm i @prisma/client
npm i bcryptjs
npm i -D @types/bcryptjs
npm i vitest vite-tsconfig-paths -D
npm i -D @vitest/ui
npm i dayjs
