<div class="markdown prose w-full break-words dark:prose-invert dark"><p>Functions in JavaScript, along with examples of how to use them:</p><ol start="5"><li>Functions<ul><li>Defining and calling functions:</li></ul><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-scss">function <span class="hljs-built_in">sayHello</span>() {
    console<span class="hljs-selector-class">.log</span>("Hello!");
}
<span class="hljs-built_in">sayHello</span>(); <span class="hljs-comment">// Output: "Hello!"</span>
</code></div></div></pre><ul><li>Function parameters and arguments:</li></ul><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">function</span> <span class="hljs-title function_">greet</span>(<span class="hljs-params">name</span>) {
    <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-string">"Hello, "</span> + name + <span class="hljs-string">"!"</span>);
}
<span class="hljs-title function_">greet</span>(<span class="hljs-string">"John"</span>); <span class="hljs-comment">// Output: "Hello, John!"</span>
</code></div></div></pre><ul><li>Anonymous functions and arrow functions:</li></ul><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-comment">// Anonymous function</span>
<span class="hljs-keyword">let</span> add = <span class="hljs-keyword">function</span>(<span class="hljs-params">a, b</span>) {
    <span class="hljs-keyword">return</span> a + b;
}
<span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-title function_">add</span>(<span class="hljs-number">2</span>, <span class="hljs-number">3</span>)); <span class="hljs-comment">// Output: 5</span>

<span class="hljs-comment">// Arrow function</span>
<span class="hljs-keyword">let</span> <span class="hljs-title function_">multiply</span> = (<span class="hljs-params">a, b</span>) =&gt; {
    <span class="hljs-keyword">return</span> a * b;
}
<span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-title function_">multiply</span>(<span class="hljs-number">2</span>, <span class="hljs-number">3</span>)); <span class="hljs-comment">// Output: 6</span>
</code></div></div></pre></li></ol><p>It's worth noting that you can define a function without a name, these are called anonymous functions, you can assign them to a variable or pass them as an argument to another function.
Arrow functions are a shorthand syntax for anonymous functions, they are also known as fat arrow functions.</p><p>Also, when a function has no explicit return value, it returns undefined by default.</p></div>