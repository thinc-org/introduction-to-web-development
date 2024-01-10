---
theme: ./theme
class: text-center
highlighter: shikiji
lineNumbers: false
drawings:
  persist: false
transition: slide-left
title: Introduction to Web Development
mdc: true
hideInToc: true
---

# Introduction to Web Development

Basic you need to know before you start your journey.

<Footer />

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
layout: statement
hideInToc: true
---

<ThincLogo class="size-64"/>
# Thailand Incubator Club

---
layout: statement
hideInToc: true
---

# Impact we made

---
hideInToc: true
layout: center
---



<div class="grid grid-cols-3 gap-2">
  <div class="justify-self-center">
    <img src="https://github.com/thinc-org/.github/raw/master/profile/assets/cupb-logo.png">
  </div>

  <div class="col-span-2">
    <h1 class="font-bold">CU Pop Bus (Deprecated)</h1>
    <p align="center">
      Never get lost in Chula again! Chula Pop Bus App helps make navigation through Chulalongkorn University much easier.
    </p>
  </div>
</div>

---
hideInToc: true
layout: center
---

<div class="grid grid-cols-3 gap-2">
  <div class="justify-self-center">
    <a href="https://book.cusc.chula.ac.th">
        <img src="https://github.com/thinc-org/.github/raw/master/profile/assets/cusc-logo.png">
    </a>
  </div>

  <div class="col-span-2">
    <h1 class="font-bold">CU Sports Center</h1>
    <p align="center">
      Tired of running to the sports center early every day? Now, you can book your court reservations anywhere at anytime.
    </p>
  </div>
</div>

---
hideInToc: true
layout: center
---


<div class="grid grid-cols-3 gap-2">
  <div class="justify-self-center">
    <a href="https://cugetreg.com">
        <img src="https://github.com/thinc-org/.github/raw/master/profile/assets/cgr-logo.png">
    </a>
  </div>

  <div class="col-span-2">
    <h1 class="font-bold">CU Get Reg</h1>
    <p align="center">
        Have no idea what courses to take? Don't know what this course is about? We got it covered. With CU Get Reg, we put all kinds of course data together so that you don't have to.
    </p>
  </div>
</div>


---
hideInToc: true
layout: center
---

# CEDT Portal Internship

<div class="grid grid-cols-2 gap-2 items-center">
  <img src="/image/cedt-home.png" alt="cedt-home" width="450">
  <img src="/image/cedt-fav-pos.png" alt="cedt-home" width="450">
</div>

---
hideInToc: true
---

# MCV Next Gen

---


<div class="m-auto w-auto h-full flex justify-center items-center flex space-x-8 items-center">
  <div>
    <img src="https://avatars.githubusercontent.com/u/33742791?v=4" class="rounded-full size-65" alt="">
  </div>

  <div>
    <h1 class="text-2xl font-bold">Saenyakorn Siangsanoh</h1>
    <div class="text-xl">Thinc. #7, CP 46</div>
    <div class="text-xl flex items-center"><strong class="mr-2">Software Engineer</strong> At <a style="border-style:none" href="https://softnetics.tech" target="_blank"><Softnetics class="ml-2 w-56 h-auto"/></a></div>
  </div>
</div>

<Footer/>


---

<div class="m-auto w-auto h-full flex justify-center items-center flex space-x-8 items-center">
  <div>
    <img src="https://avatars.githubusercontent.com/u/50145654?v=4" class="rounded-full size-65" alt="">
  </div>

  <div>
    <h1 class="text-2xl font-bold">Supakarin Niansupornpun</h1>
    <div class="text-xl">Thinc. #9, CP 48</div>
    <div class="text-xl flex items-center slidev-vclick-target"><strong class="mr-2">President</strong> of <a style="border-style:none" href="https://thinc.in.th" target="_blank"><ThincLogo class="ml-2 w-36 h-auto pb-2"/></a></div>
  </div>
</div>

<Footer/>

---
hideInToc: true
---

# Table of contents

<Toc columns="3" />

<Footer/>

---

# Begin of Web Development

<div class="flex w-full pt-4 items-center justify-center space-x-12">
  <img width="200"  src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Netscape_icon_2007.svg/1200px-Netscape_icon_2007.svg.png" alt="netscape" />

  <img width="350" src="https://www.zdnet.com/a/img/2014/10/20/79e0c246-5840-11e4-b6a0-d4ae52e95e57/netscape1.jpg" alt="netscape" />
</div>

<Footer/>

---

# What is Browser

**Browser** is **application program** that provides a way to look at and interact with all the information on the World Wide Web.

<div class="bg-white">
  <img src="/assets/browser.png" alt="" />
</div>

---

# Actual network scenario

FYI, you don't have to know all of this.

<img src="/assets/actual-network.png" alt="" class="h-[400px]" />

---

# After browser get content (DOM)

Browser will take HTML to construct **DOM (Document Object Model)**.

```html {all|6-7}
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link ref="stylesheet" href="LINK" />
    <script type="text/javascript" src="LINK"></script>
    <title>Document</title>
  </head>
  <body>
    <h1>Hello World</h1>
  </body>
</html>
```

---

# Stylesheet (CSS)

Browser will take CSS to construct **CSSOM (CSS Object Model)**.

```css
h1 {
  color: red;
}
```

# JavaScript (JS)

```js
function onClick() {
  alert("Hello World");
}

document.querySelector("h1").addEventListener("click", onClick);
```

---
layout: image-right
image: https://miro.medium.com/v2/resize:fit:4800/format:webp/1*ejR8TwuRBqTRDKmAJeltig.png
---

# HTML, CSS, JS parsing

Reference: 

- https://web.dev/articles/howbrowserswork
- https://web.dev/articles/critical-rendering-path/constructing-the-object-model
- https://javascript.plainenglish.io/web-performance-understanding-critical-rendering-path-72283caefc1f

---

# N-tier Architecture

<div class="bg-white">
  <img src="/assets/architecture.png" alt="" />
</div>

---

# Web Evolution

<img src="https://www.goodrequest.com/_next/image?url=https%3A%2F%2Fgoodrequest-web.s3.eu-central-1.amazonaws.com%2FHistory_of_web_Web_1_0_3_0_8124a4915c.png&w=3840&q=75" alt="" class="h-[400px]" />

---

# Web 1.0

The customer can not edit the content that the website provides which means that **the customer can only read the content**.

### Keyword

- **One-way communication**
- **Read**

### Example

- News website
- Wikipedia
- etc.

---

# Web 2.0

The customer can interact with the website by **editing the content**. The website will be updated in real-time which leads to the **growth of social media**.

### Keyword

- **Two-way communication**
- **Read-Write**

### Example

- Facebook
- Twitter
- Instagram
- etc.

---

# Web 3.0

As the internet grows, the amount of data that the website has to handle is increasing. **Web 3.0** is the solution to this problem. It is the **decentralized web** that uses **blockchain** to store data. We might don't want to trust the third party to store our data.

### Keyword

- **Decentralized**
- **Read-Write-Trust**

### Example

- PancakeSwap
- Uniswap

---

# Server Side Rendering (SSR)

---

# Client Side Rendering (CSR)

---

# SSG, ISR, RSC and more

---

# Old School Web Development

1. PHP
2. JAVA
3. Ruby on Rails

---

# Web Frameworks

## Why do we need it?

--- 

# React

---

# NextJS

---

# Full Stack Web Development

---

# Back to Basics

## "use server"

---

# Do we need backend?

---

# Backend Purpose

---

# Backend Paradigms

1. Monolithic
2. Microservice
3. Serverless
4. Etc.

---
layout: statement
---

# Backend Languages

<h3 v-click>
 You can use any language you want
</h3>

---

# Backend Frameworks in 2023 - 2024

---

# Version Control System (VCS)

---

# Git

---

# Dev(Sec)Ops

---

# Docker

---

# Kubernetes

---

# GitOps

--- 

# Cloud Providers

---

# Clean Code

- Naming
- Commenting
- SOLID
- KISS (Keep It Simple Stupid)

---

# Software Architecture

---

# Software Design Patterns

---

# Find your passion
