# highlightjs-riscvasm - RISC-V grammar for highlight.js

## Usage

### Static website

Simply load the module after loading Highlight.js:
```html
<link rel="stylesheet" href="/path/to/styles/default.min.css">
<script src="/path/to/highlight.min.js"></script>
<script src="/path/to/riscvasm.min.js">
<script>hljs.highlightAll();</script>
```

There is a esm style to use it:
```html
<link rel="stylesheet" href="/path/to/styles/default.min.css">
<script type="module">
    import hljs from '/path/to/highlight.min.js';
    import riscvasm from '/path/to/riscvasm.es.min.js';
    hljs.registerLanguage('riscv', riscvasm);
    hljs.highlightAll();
</script>
```

Your html may look like:
```html
<pre><code class="language-riscv">
    ...
</code></pre>
```

### ES6 Module

It can be imported as a module, then register it. CommonJS also works in the same way.

```javascript
import hljs from 'highlight.js';
import riscvasm from 'highlightjs-riscvasm';

hljs.registerLanguage("riscv", riscvasm);
hljs.highlightAll();
```

Your html may look like:
```javascript
<pre><code class="language-riscv">
    ...
</code></pre>
```