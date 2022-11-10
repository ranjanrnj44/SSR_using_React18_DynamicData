# Required Tools:

1. Any prefered IDE , nodejs installed, Chrome browser

# Some other tools I used

1. Express : (Implemented Routings)
2. Nodejs : (Read/Write file using FileSystem, Streams)

# Objective

Performance optimisation with 0 loading time and SEO Optimized - Certain part of the page's load time can be increased using React18's new feature(renderToPipebleStream). At initial load users instead of seeing blank page they can see the actual layout with pre-fetched contents.

# SSR in React 18

THis application is developed using React18 feature (renderToPipebleStream - to attain SSR feature).

# How to setup and Run the Project

To obtain SSR, we need to create react script to build client side scripts

- npm run build
- npm run ssr

# NOTE (Routing path) :

I have provided 2 routes (/test , /apicall) please use the path

1. /test - It has a simple json file.
2. /apicall - This makes 2 api call on server and pass those data to client side.

# Any Blocker/Got Stuck?, Remember this points to check

1. Hydration issue - Remember, our SSR(build/index.html) and CSR(public/index.html) file should match with same data, if not we will get app crash.
2. Don't use renderToString(it does not support streaming, lazy loading). It comes with less supported use only.

# Reference

SSR DOCS :

1. Understanding React 18 Architecture :
   https://blog.saeloun.com/2022/01/20/new-suspense-ssr-architecture-in-react-18
   https://github.com/reactwg/react-18/discussions/37
   https://blog.saeloun.com/2021/12/16/hydration
   https://reactjs.org/docs/react-dom-server.html#rendertopipeablestream
2. CSR vs SSR :
   https://ts.accenture.com/:w:/s/InnovationTeam187/EdnNHs7ji_FAvzL1JxYSIg4BAqEaEMI3dq8XW0-LcSh1LQ?e=zwbTQA
3. Upgrading R18 on server :
   https://github.com/reactwg/react-18/discussions/22

SSR VIDEO :

1. Streaming Server Rendering with Suspense : https://www.youtube.com/watch?v=pj5N-Khihgc
2. React 18 Features : https://www.youtube.com/watch?v=Z-NCLePa2x8&t=1s

OTHER REFERENCE

1. Suspense (for data fetching - EXPERIMENTAL) :
   https://dev.to/darkmavis1980/a-practical-example-of-suspense-in-react-18-3lln
