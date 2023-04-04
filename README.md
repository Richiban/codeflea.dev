# codeflea.dev

_A statically generated blog example using Next.js, Markdown, and TypeScript_

> Note: this is the code for the website `codeflea.dev`. If you're looking for the code for the VS Code extension itself, [click here](https://github.com/Richiban/codeflea).

This makes use of Next.js's [Static Generation](https://nextjs.org/docs/basic-features/pages) feature using Markdown files as the data source.

The blog posts are stored in `/_posts` as Markdown files with front matter support. Adding a new Markdown file in there will create a new post.

To create the blog posts we use [`remark`](https://github.com/remarkjs/remark) and [`remark-html`](https://github.com/remarkjs/remark-html) to convert the Markdown files into an HTML string, and then send it down as a prop to the page. The metadata of every post is handled by [`gray-matter`](https://github.com/jonschlinkert/gray-matter) and also sent in props to the page.

## How to use

Clone the repo, run

```bash
npm install
```

and then

```bash
npm run dev
```

The site should be up and running on [http://localhost:3000](http://localhost:3000)!

It deploys to the cloud with [Vercel](https://vercel.com/new?utm_source=github&utm_medium=readme&utm_campaign=next-example) ([Documentation](https://nextjs.org/docs/deployment)).

# Notes

`codeflea.dev` uses [Tailwind CSS](https://tailwindcss.com) [(v3.0)](https://tailwindcss.com/blog/tailwindcss-v3).
