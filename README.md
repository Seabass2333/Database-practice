This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

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

> create an .env file copied from .env.example

### MySQL
##### database
> aiven: https://console.aiven.io/
> add DATABASE_URL to .env
> change ./prisma/schema.prisma file content
> run `npx prisma generate`
> run `npx prisma db push`, it might be get an error something like `Can't reach database server at ...`, it's because aiven database isn't ready, just waiting a few minutes and run it again
> run `npx prisma studio`, you will see the table of database

### PostgreSQL
##### database
> Neon: https://console.neon.tech/app/projects
> change ./prisma/schema.prisma file content
> run `npx prisma generate`
> run `npx prisma db push`, it's much faster than aiven
> run `npx prisma studio`, you will see the table of database, or you can edit database in the neon site directly

### MOngoDB
##### database 
> MongoDB: https://cloud.mongodb.com/v2
> change ./prisma/schema.prisma file content
> run `npx prisma generate`
> run `npx prisma db push`
> run `npx prisma studio`, you will see the table of database