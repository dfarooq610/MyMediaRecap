# MyMediaRecap

in 2023, i want to be able to share an instragram story highlighting what i watched, listened to, and read each month. This is a tool to try and generate those images programatically, since designing them manually in figma was quite a pain.

given a list of IMDB movie IDs and a list of LCCN Book Numbers, and a background color hex code generates an 1080x1920 image to share on instagram

### Input
```json
{
  "movies": ["tt19770238", "tt3915174"],
  "books": ["2020022471"],
  "background": "02534C",
}
```

### Output
<p align="center">
  <img src="https://user-images.githubusercontent.com/59672089/215275423-97e4b2e1-4357-4d30-856e-8de6a14939be.png" width="324" height="576">
</p>

### Features
- ideally fetches top tracks from spotify API for your user. 

- for movie thumbnails, uses https://www.omdbapi.com/

- for book thumbnail, uses https://openlibrary.org/dev/docs/api/covers

- need to think of a programatic way to generate the pic of the month. Want assets to autoscale within boundaries (what if i had 7 movies?)

- need to think of a way to analyze the book of the month

- might be nice to make a UI where you can directly share to instagram stories?

### etc
This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.tsx`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.ts`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
