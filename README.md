# highlightjs-riscvasm - RISC-V grammar for highlight.js

## Usage

### ES6 Module

Also can import it as a module, then register it. CommonJS also works in the same way.

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