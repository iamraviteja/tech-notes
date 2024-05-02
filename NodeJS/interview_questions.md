1) What is the difference between Bun, NodeJS and Deno
Both Node.js and Bun are runtimes. Node.js is primarily written in C++ where as Bun is written with a low-level general purpose programming language called Zig. But that is just the tip of the ice berg. Let’s take a closer look at other differences when treating Bun as a runtime alone.
===============================
2) What is the difference between javascript runtime and javascript engine
A JavaScript runtime is an environment which provides all the necessary components in order to use and run a JavaScript program.

A JavaScript engine is a program that converts JavaScript code we write into machine code that allows a computer to perform specific tasks.

While Node.js uses Google's V8 engine that power's Chrome browser, Bun uses JavaScriptCore (JSC), which is an open source JavaScript engine developed by Apple for Safari.

V8 and JSC have different architectures and optimization strategies. JSC prioritizes faster start times and reduced memory usage with a slightly slower execution time. On the other hand, V8 prioritizes fast execution with more runtime optimization which may lead to more memory usage.

This makes Bun fast, starting up to 4x faster than Node.js.
===============================
What is the difference between CommonJS and ES6 Modules
https://www.syncfusion.com/blogs/post/js-commonjs-vs-es-modules

what is tree shaking?

What is the javascript engine used by nodejs, What are some other javascript engines?
1. V8 – JavaScript Engine developed by Google for Chrome
2. SpiderMonkey – The JavaScript Engine used by Mozilla Firefox
3. JavaScriptCore – Developed by Apple for Safari
4. Rhino – Managed by Mozilla Foundation for Firefox
5. Chakra – A JavaScript Engine for Microsoft Edge

How do we pull packages from custom repository rather that npm registry
We can specify the repository in .npmrc file

What is other use of .npmrc file

What is the difference between commonjs and es modules.

How would you indicate to node to use es modules
In package.json set type=module

What is event loop in nodejs

What is the difference between setImediate and process.nextTick()
What is the difference between micro task and macro task

What is an event emitter in node js
How to code Observable in node js

What are streams in nodejs, what are different types of streams ?
What is the use of streams?

Expressjs questions


Reference Links:
https://www.builder.io/blog/bun-vs-node-js
https://www.freecodecamp.org/news/javascript-engine-and-runtime-explained/
https://algodaily.com/lessons/introduction-to-js-engines-and-runtimes