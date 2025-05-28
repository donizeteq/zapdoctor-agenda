This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.

---

# Clinica Agenda - Sistema de Agendamento para Clínicas

## Visão Geral

O Clinica Agenda é um sistema web desenvolvido com Next.js 15 para gerenciamento e agendamento de consultas médicas. O projeto utiliza uma arquitetura moderna com React 19, TypeScript, Tailwind CSS e Drizzle ORM para persistência de dados em PostgreSQL.

## Tecnologias Utilizadas

### Frontend

- Next.js 15.3.2 : Framework React com renderização híbrida (SSR/CSR)
- React 19.0.0 : Biblioteca para construção de interfaces
- TypeScript : Superset tipado de JavaScript
- Tailwind CSS 4 : Framework CSS utilitário
- Shadcn UI : Componentes de UI baseados em Radix UI
- React Hook Form : Gerenciamento de formulários
- Zod : Validação de esquemas e tipagem

### Backend

- Next.js API Routes : Endpoints da API
- Drizzle ORM : ORM para PostgreSQL
- PostgreSQL : Banco de dados relacional

## Estrutura do Projeto

```
├── src/
│   ├── app/                  # Rotas e 
páginas da aplicação
│   │   ├── authentication/   # 
Autenticação (login/registro)
│   │   ├── globals.css       # Estilos 
globais
│   │   ├── layout.tsx        # Layout 
principal
│   │   └── page.tsx          # Página 
inicial
│   ├── components/           # Componentes 
reutilizáveis
│   │   └── ui/               # Componentes 
de interface
│   ├── db/                   # 
Configuração do banco de dados
│   │   ├── index.ts          # Conexão com 
o banco
│   │   └── schema.ts         # Esquema do 
banco de dados
│   └── lib/                  # Utilitários 
e funções auxiliares
│       └── utils.ts          # Funções 
utilitárias
```

## Modelo de Dados

O sistema gerencia as seguintes entidades principais:

- Usuários : Contas de acesso ao sistema
- Clínicas : Estabelecimentos médicos
- Médicos : Profissionais com especialidades e horários disponíveis
- Pacientes : Clientes das clínicas
- Agendamentos : Consultas marcadas entre médicos e pacientes

## Funcionalidades

### Implementadas

- Sistema de autenticação (registro de usuários)
- Interface com design responsivo usando Tailwind CSS
- Validação de formulários com React Hook Form e Zod

### Em Desenvolvimento

- Login de usuários
- Gerenciamento de clínicas
- Cadastro de médicos e pacientes
- Agendamento de consultas
- Dashboard administrativo

## Configuração do Ambiente de Desenvolvimento

### Pré-requisitos

- Node.js (versão recomendada: 20.x ou superior)
- PostgreSQL

### Instalação

1. Clone o repositório

```
git clone [url-do-repositorio]
cd clinica-agenda
```

2. Instale as dependências

```
npm install
```

3. Configure as variáveis de ambiente
   Crie um arquivo .env na raiz do projeto com as seguintes variáveis:

```
DATABASE_URL=postgresql://
usuario:senha@localhost:5432/clinica_agenda
```

4. Execute as migrações do banco de dados

```
npx drizzle-kit push
```

5. Inicie o servidor de desenvolvimento

```
npm run dev
```

6. Acesse a aplicação em http://localhost:3000

## Scripts Disponíveis

- npm run dev : Inicia o servidor de desenvolvimento
- npm run build : Compila o projeto para produção
- npm start : Inicia o servidor em modo de produção
- npm run lint : Executa a verificação de linting

## Estilo e Design

O projeto utiliza o tema "New York" do Shadcn UI com suporte a modo claro e escuro. A fonte principal é Geist, otimizada para legibilidade em interfaces web.

## Aprenda Mais

Para saber mais sobre Next.js, consulte os seguintes recursos:

- Documentação do Next.js - aprenda sobre os recursos e API do Next.js.
- Aprenda Next.js - um tutorial interativo de Next.js.

## Deploy na Vercel

A maneira mais fácil de implantar seu aplicativo Next.js é usar a Plataforma Vercel dos criadores do Next.js.

Consulte nossa documentação de implantação do Next.js para mais detal.
