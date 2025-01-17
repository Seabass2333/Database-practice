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

1. aiven: https://console.aiven.io/
2. add DATABASE_URL to .env
3. change ./prisma/schema.prisma file content
4. run `npx prisma generate`
5. run `npx prisma db push`, it might be get an error something like `Can't reach database server at ...`, it's because aiven database isn't ready, just waiting a few minutes and run it again
6. run `npx prisma studio`, you will see the table of database

### PostgreSQL

##### database

1. Neon: https://console.neon.tech/app/projects
2. change ./prisma/schema.prisma file content
3. run `npx prisma generate`
4. run `npx prisma db push`, it's much faster than aiven
5. run `npx prisma studio`, you will see the table of database, or you can edit database in the neon site directly

### MOngoDB

##### database

1. MongoDB: https://cloud.mongodb.com/v2
2. change ./prisma/schema.prisma file content
3. run `npx prisma generate`
4. run `npx prisma db push`
5. run `npx prisma studio`, you will see the table of database


**PS: please check out the details about every type of database in different branches!**