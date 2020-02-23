---
layout: post
title: Tech Evaluation
date: 2020-02-20T13:50:44.908Z
---

Comparison of **React/Gatsby** vs **Svelte/Sapper** 

## Problem statement

- Need blazing fast CMS based website performance
- Easy to code and maintain with additional advantage of lesser JS build size
- CDN-ready js/html bundle
- Should be able to integrate with an existing CMS
- The website may contain complex UI components like Google Map

---

## React with Gatsby

#### Pros
- Provides CMS integration by default, Support for `WordPress`, `Drupal`
- Uses `GraphQL` to fetch data from CMS or APIs
- Builds your site as "static" files which can be deployed easily on dozens of services
- Real cases of improved `Google PageSpeed score` after adopting gatsby.js by big sites
- Server-Side rendering, route based Code-splitting

{% include image.html path="gatsby.svg" 
 path-detail="gatsby.svg"
 alt="Gatsby" %}

#### Cons
- Dependency on `React`, `GraphQL`

---

## Svelte with Sapper

#### Pros
- Minimum bundle size compared to React/Vue/Angular
- Svelte is a compiler-as-framework
- Compiles components down at the build step, allowing you to load a single bundle.js on your page to render your app.
- No virtual DOM, no frameworks on top of frameworks, and no framework to load at runtime
- Growing community in Svelte
- Code-splitting, offline support

#### Cons

- Fairly newer compiler/fw
- No CMS integration by default
- Need to add a layer to fetch the data from CMS 
    (can refer this [blog](https://kyleadkins.design/how-i-built-this-website-with-svelte-and-the-wordpress-rest-api) which demonstrates how wordpress can be integrated)
- Sapper currently at `v0.26`, which is in early development
