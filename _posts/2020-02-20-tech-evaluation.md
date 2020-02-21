---
layout: post
title: Tech Evaluation
date: 2020-02-20T13:50:44.908Z
---

Blazingly fast CMS based website 

## Problem statement

- Need blazing fast CMS based website performance
- Easy to code and maintain with additional advantage of lesser JS build size
- CDN-ready js/html bundle
- Should be able to integrate with an existing CMS
- The website may contain complex UI components like Google Map

---

## Gatsby

#### Pros
- Provides CMS integration by default
  - Support for `WordPress`, `Drupal`
- Uses `GraphQL` to fetch data from CMS or APIs
- Builds your site as "static" files which can be deployed easily on dozens of services
- Real cases of improved `Google PageSpeed score` after adopting gatsby.js by big sites

{% include image.html path="gatsby.svg" 
 path-detail="gatsby.svg"
 alt="Gatsby" %}

#### Cons
- Dependency on `React`, `GraphQL`

---

## Svelte

#### Pros
- Svelte is a compiler-as-framework
- Compiles components down at the build step, allowing you to load a single bundle.js on your page to render your app.
- No virtual DOM, no frameworks on top of frameworks, and no framework to load at runtime

#### Cons

- Fairly newer compiler/fw
- No CMS integration by default
- Need to add a layer to fetch the data from CMS
