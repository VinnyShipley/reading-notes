# React 4

## Dynamic Routes

Dynamic paths are pages that statically generate pages with paths dependent on external data.

To create a dynamic path:

Name the page that you want to be dynamic with square brackets around the filename. That page must contain:

    * A React component to render the page

    * getStaticPaths which returns an array of possible values for id (id in this case being the name of the file)

    * get Static Props which fetches the necessary data for the post with id

## Deploying Your Next.js App

To deploy your Next.js app:

* Push to github

* Deploy to Vercel (This usually goes smoothly as the creators of Next.js created Vercel)