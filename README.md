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

## [My-notes]

You can move the Primary Side Bar to the right hand side by right-clicking the Activity Bar and selecting Move Primary Side Bar Right or toggle its visibility (Ctrl+B).

changes happened to setting json of vscode

[alt+z] to wrap code lines

change slogans in lib/constants.ts and .env.local
change category array inside search.tsx to array from database
inside header/index.tsx ==> <Button variant='ghost' means the button bg is transparent
made a humburger menu icon (shadcdn) inside a button .
also showed the links in the hearder using map funtion which is a better way to do it.
in header/index.tsx <div className='hidden md:block flex-1 max-w-xl'>
<Search />

</div>
<Menu /> (sign in , cart)
</div>
<div className='md:hidden block py-2'>
<Search />
</div> means, on small screen search will be after menu ==> on big screen search will be before menu

to open new tab in vscode ==> code . ==> it has to have space between.

ctrl c to get out of the running terminal.

---

only limit network access of mongodb to varcel and my laptop.

---

```js
ratingDistribution: z
  .array(
    z.object({
      rating: z.number(),
      count: z.number(),
    })
  )
  .max(5),
```

```js
z.array(...):
```

This defines an array schema. It means ratingDistribution is expected to be an array.

```js
z.object({ ... }):
```

This defines the structure of each object in the array. Each object must have two properties:

rating: A number.

count: A number.

```js
rating: z.number():
```

The rating property must be a number.

```js
count: z.number():
```

The count property must also be a number.

```js
.max(5):
```

This adds a validation rule to the array. It ensures that the array has a maximum length of 5. If the array has more than 5 elements, validation will fail.

## Dealing with teh [database] [mongodb]:

make a project , then make a cluster0 [free], browse collections ==> will show database with all collections under it ==> here you can create databases or the sub databases [which-called-collections].

---

---

## --------------------- changing any keys of the input of a product --------

lib\validator.ts
lib/data.ts
lib\db\models\product.model.ts

commented colors key to the three files
added form key to all three files
changes the value of brands to EV in the data.ts file
