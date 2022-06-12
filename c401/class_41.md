# React 4

## Dynamic Routes

Dynamic Routes - allows for page generation per id 

create a page called [id].js under pages/posts

Steps:

- Create a react component to render the page
- getStaticPaths returns array of objects
- getStaticProps fetches data for post with id

```js
import Layout from '../../components/layout';


export default function Post() {
  return <Layout>...</Layout>;
}

export async function getStaticPaths() {
  // Return a list of possible value for id
}

export async function getStaticProps({ params }) {
  // Fetch necessary data for the blog post using params.id
}

```

[dynamic-routes walkthough](https://nextjs.org/learn/basics/dynamic-routes)

## Deployment

How to deploy your nextjs app on Vercel

vercel is made by the creators of Nexjs!

Things versel handdles for your

- Static generation assets auto serve form Vercel Edge network
- Server-Side Rendering and API routes automatically become serverless functions

Other Vercel Features

- Custom Domains
- Set Environment Variables
- Automatic HTTPS configuration


[nextjs Deployment](https://nextjs.org/learn/basics/deploying-nextjs-app)
