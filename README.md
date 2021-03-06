# Eleventy + Stylus Blog theme

[![Netlify Status](https://api.netlify.com/api/v1/badges/a180e099-11d2-49d4-9697-910d56980343/deploy-status)](https://app.netlify.com/sites/reverent-carson-67c52e/deploys)
[![Build Status](https://travis-ci.com/villivald/create-react-app-blog.svg?branch=main)](https://travis-ci.com/villivald/create-react-app-blog)
[![Vercel Status](https://vercel-badge-ar363.vercel.app/?app=eleventy-stylus-blog-theme)](https://github.com/villivald/create-react-app-blog/deployments/activity_log?environment=Production)

[Speedlify](https://crappblog.netlify.app/)

A theme repository that contains a blog built with [Eleventy](https://github.com/11ty/eleventy) and [Stylus](https://stylus-lang.com/)

## Features

- 100% Lighthouse scores
- Toggleable dark theme (PS. theme preference is also stored in `localStorage`)
- Tags as taxonomy
- Stylus CSS preprocessor
- Integrated with Eleventy's official [navigation plugin](https://www.11ty.dev/docs/plugins/navigation/)
- Also generates Atom RSS Feed with Eleventy's official [RSS plugin](https://www.11ty.dev/docs/plugins/rss/)
- Sitemap generation
- Non-post pages support (eg. About page, Contact page)
- Modular type scale implemented in with Stylus

## Demos

- Vercel: https://create-react-app-blog.vercel.app/
- Netlify: https://reverent-carson-67c52e.netlify.app/

## Screenshots

## Deploy this template to your own site

Get your site up and running with a few clicks

- [Deploy on Netlify](https://app.netlify.com/start/deploy?repository=https://github.com/ar363/eleventy-stylus-blog-theme)
- [Deploy on Vercel](https://vercel.com/import/project?template=ar363%2Feleventy-stylus-blog-theme)

## Getting started locally

1. Clone this repo

```
git clone https://github.com/ar363/eleventy-stylus-blog-theme my-blog
```

2. Navigate to the blog directory

```
cd my-blog
```

3. Install dependencies with [yarn](https://yarnpkg.com/)

```
yarn
```

4. Edit `_data/site.js` according to your site preferences

5. Also optionally modify `stylus/abstracts/variables.styl` according to your preference

To watch for changes in Eleventy and Stylus, use `yarn dev`

To build without watching for changes, use `yarn build`
