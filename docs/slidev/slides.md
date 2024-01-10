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

---
src: ./pages/intro.md
hideInToc: true
---

---
layout: statement
hideInToc: true
---

# Impact we made

---
src: ./pages/impact-we-made/cu-pop-bus.md
hideInToc: true
---

---
src: ./pages/impact-we-made/sport-complex.md
hideInToc: true
---

---
src: ./pages/impact-we-made/cu-get-reg.md
hideInToc: true
---

---
src: ./pages/impact-we-made/cedt-portal.md
hideInToc: true
---

---
src: ./pages/speaker/saenyakorn.md
hideInToc: true
---

---
src: ./pages/speaker/supakarin.md
hideInToc: true
---

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
layout: section
---

# What is a web browser?

And how does it work?

---
src: ./pages/what-is-browser/what-is.md
---

---
src: ./pages/what-is-browser/url-vs-uri.md
hideInToc: true
---

---
src: ./pages/what-is-browser/url.md
hideInToc: true
---

---
src: ./pages/what-is-browser/actual-network-scenario.md
hideInToc: true
---

---
layout: section
---

# How Browser render a page?

<div class="bg-white">
  <img src="/assets/browser.png" alt="" />
</div>

---
src: ./pages/browser-rendering/html.md
hideInToc: true
---

---
src: ./pages/browser-rendering/css-js.md
hideInToc: true
---

---
src: ./pages/browser-rendering/dom.md
hideInToc: true
---

---
src: ./pages/browser-rendering/cssom.md
hideInToc: true
---

---
src: ./pages/browser-rendering/crp.md
hideInToc: true
---

---
layout: section
---

# How real-world web application works?

---
src: ./pages/what-is-browser/n-tier.md
hideInToc: true
---



---
src: ./pages/evolution/intro.md
hideInToc: true
---

---
src: ./pages/evolution/web-1.md
hideInToc: true
---

---
src: ./pages/evolution/web-2.md
hideInToc: true
---

---
src: ./pages/evolution/web-3.md
hideInToc: true
---

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
layout: statement
---

# Language You Should Know in 2024

---
layout: center
---

# TypeScript

<img src="/image/ts-in-js.png" alt="ts-in-js" class="h-[400px]" />

---
layout: center
---

# JavaScript is a mess

<img src="https://res.cloudinary.com/practicaldev/image/fetch/s--ij_hqKUb--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://github.com/damiancipolat/js_vs_memes/blob/master/doc/mind_js.jpg%3Fraw%3Dtrue" alt="js-hell" class="h-[400px]" />

Credit: [Damian Cipolat](https://dev.to/damxipo/javascript-versus-memes-explaining-various-funny-memes-2o8c)

---
layout: center
---


<img src="https://www.freecodecamp.org/news/content/images/2019/07/panel-1-1.png" alt="js-hell" class="w-[800px]" />

---

# Which property is missing?

```js
function doSomething(params) {
  if (params.age > 30) {
    if (params.job === 'Developer' && params.hobby === 'Coding') {
      console.log('Experienced developer who loves coding');
    } else if (params.job === 'Designer') {
      console.log('Creative designer');
    } else {
      console.log('Professional with other interests');
    }
  } else {
    if (params.address && params.address.city === 'New York') {
      console.log('Young professional living in New York');
    } else {
      console.log('Young professional from another place');
    }
  }
}

doSomething({
  name: 'John',
  age: 20,
  job: 'Developer',
  hobby: 'Coding',
});
```

---

# TypeScript is a solution

```ts twoslash
type ParamsType = {
  name: string;
  age: number;
  job: string;
  hobby: string;
  address: string;
}

// ---cut---

function doSomething(params: ParamsType) {
  // some logic...
}

// @errors: 7006
doSomething({
  name: 'John',
  age: 20,
  job: 'Developer',
  hobby: 'Coding',
});

```

<style>
  .twoslash .twoslash-error-line {
    white-space: pre-line;
  }
</style>

---

# Power of TypeScript (eg. [tRPC](https://trpc.io))

<video autoplay="" loop="" muted="" playsinline="" width="1200px" class="rounded-lg border-4 border-neutral-900 bg-neutral-900 shadow-xl md:hidden h-[400px]" poster="https://assets.trpc.io/www/v10/preview-dark.png"><source src="https://assets.trpc.io/www/v10/preview-dark.mp4" type="video/mp4">You need a browser that supports HTML5 video to view this video.</video>

<video autoplay="" loop="" muted="" playsinline="" width="1200px" class="hidden md:block" poster="https://assets.trpc.io/www/v10/v10-dark-landscape.png"><source src="https://assets.trpc.io/www/v10/v10-dark-landscape.mp4" type="video/mp4">You need a browser that supports HTML5 video to view this video.</video>

---
layout: iframe
url: https://typehero.dev/
---

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
layout: statement
hideInToc: true
---

# The Importance Things!

---
layout: center
---

# Clean Code

<img src="https://www.freecodecamp.org/news/content/images/2020/10/clean-code-image.png" alt="clean-code" class="h-[350px]" />

Credit: Clean Code

---
level: 2
layout: center
---

# Productivity vs Time

<img src="https://1143146101-files.gitbook.io/~/files/v0/b/gitbook-legacy-files/o/assets%2F-M4CT8WYORuS-KboTDGB%2F-M4CT8x9OG0AAsbaoOFE%2F-M4CTCxSNa_0ygH32IuE%2Fproductivity-vs-time.jpg?generation=1586142727262504&alt=media" alt="productivity-graph" class="h-[350px]" />
Credit: Clean Code

---
level: 2
layout: center
---

# Cost vs Time

<img src="/image/cost-graph.png" alt="cost-graph" class="h-[350px]" />


---
layout: center
---

<img src="/image/big-refactor.png" class="h-300px"/>

---
level: 2
layout: center
---


```java 
for (int j = 0; j < 34; j++) {
  s += (t[j] * 4) / 5;
}
```

<center class="py-4">vs</center>

```java 
final int realDaysPerIdealDay = 4;
final int WORK_DAYS_PER_WEEK = 5;
final int NUMBER_OF_TASKS = 34;
int sum = 0;
for (int j = 0; j < NUMBER_OF_TASKS; j++) {
  int realTaskDays = taskEstimate[j] * realDaysPerIdealDay;
  int realTaskWeeks = (realTaskDays / WORK_DAYS_PER_WEEK);
  sum += realTaskWeeks;
}
```

---
level: 2
layout: center
---

# SOLID

<img src="https://blog.m2pfintech.com/wp-content/uploads/2023/06/Solid-Principle-Blog-2nd-Banner.jpg" alt="solid" class="h-[400px]" />

Credit: [M2P Fintech](https://m2pfintech.com/blog/solid-principles-a-comprehensive-guide-to-object-oriented-programming-and-class-design-using-swift/)

---
level: 3
---

# Single Responsibility Priciple

Without SRP

```ts
class Reporter {
    constructor(private title: string, private content: string) {}

    generateReport(): void {
        // Code for generating the report
        // ...
    }

    saveToFile(filePath: string, exportType: 'pdf' | 'html'): void {
        if (exportType === 'pdf') {
            // Code for exporting as PDF
            // ...
        } else if (exportType === 'html') {
            // Code for exporting as HTML
            // ...
        }
    }
}
```

---
hideInToc: true
---

# Single Responsibility Priciple

With SRP

```ts
class Reporter {

    constructor(private title: string, private content: string, private formatter: Formatter) {}

    generateReport(): string {
        // Code for generating the report
        const formattedContent = this.formatter.formatContent(this.content);
        return formattedContent;
    }
}

interface Formatter {
    formatContent(content: string): string;
}

class HTMLFormatter implements Formatter {
    formatContent(content: string): string {
        // Code for formatting content as HTML
        // ...
        return "HTML formatted content";
    }
}

class PDFFormatter implements Formatter {
    formatContent(content: string): string {
        // Code for formatting content as PDF
        // ...
        return "PDF formatted content";
    }
}

class ReportSaver {
    saveToFile(content: string, filePath: string): void {
        // Code for saving the report to a file
        // ...
    }
}
```

<style>
  pre {
    max-height: 400px;
  }
</style>

---
hideInToc: true
layout: two-cols
---

# More About Clean Code

- Naming
- Comment
- Function
- Class
- KISS (Keep It Simple Stupid)
- DRY (Don't Repeat Yourself)
- Software Architecture (eg. MVC, MVVM, Clean Architechture etc.)
- **Unit Test**
- **TDD**

::right::

<img src="https://m.media-amazon.com/images/W/MEDIAX_792452-T1/images/I/51E2055ZGUL._SL1000_.jpg" alt="clean-code-book" class="h-[500px]"/>

---
layout: quote
---

<strong class="text-[48px]">"The only way to go fast is to go well"</strong>
Uncle Bob

---
layout: quote
---

<Tweet id="1163789159309434880"/>

---
layout: center
---

# Agile is about code

---

# Find your passion
