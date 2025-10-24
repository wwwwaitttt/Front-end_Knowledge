# What is the function of the parameters preload and prefetch of the html rel attribute

## foreword 

`rel` attribute is used `<link>`tag that defines the relationship to the current document. `preload` and `prefetch` are two important parameters that are resource loading optimization tools to improve web page performance and user experience. Understanding their differences and applications is helpful for rational planning of resource loading sequence. 

## The role and difference between preload and prefetch 

**preload** used to tell the browser to load critical resources as early as possible, such as fonts, key scripts, styles, or images, that are needed immediately when the current page is rendered. `preload` provide priority prompt, the browser will get resources as soon as possible to avoid rendering blocking.

Example of use: 
```HTML
<link rel="preload" href="main.css" as="style">
```
**prefetch** used to tell the browser to load resources that may be used in the future, usually used to navigate to the next page. It has a lower priority, and the browser will download it when it is idle to avoid blocking the current page resource load. 

Example of use: 
```HTML
<link rel="prefetch" href="next-page.js">
```
the difference is: 

- preload is the current page needs immediately, with priority loading.
- prefetch is likely to be needed in the future, lazy loading. 

The combination of the two can improve the initial loading speed of the page and the subsequent page switching experience. 

## Application Scenarios 

- preload commonly used in key CSS, JS, fonts and other resources to optimize the first screen rendering. 
- prefetch it is used to preload the next page resource that the user may visit, improving the response speed. 

## Interview answer 
`rel="preload"` it is used to inform the browser to load the key resources of the current page first to ensure the fast rendering of the page; `rel="prefetch"` it is used to prompt the browser to pre-load resources that may be needed in the future when it is idle to improve subsequent access performance. The difference between the two is that the priority and loading time are different, and reasonable use helps to improve the performance of the web page. 

## Summary 

`preload` and `prefetch` it is an important tool for front-end performance optimization. It helps browsers reasonably schedule network requests for current key resources and future potential resources, and improves user experience. Understanding and using them correctly is an indispensable skill for modern front-end development.