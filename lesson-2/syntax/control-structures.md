<div class="markdown prose w-full break-words dark:prose-invert light"><p>Control structures in JavaScript, along with examples of how to use them:</p><ol start="5"><li>Control Structures<ul><li>Conditional statements:<ul><li>if: Executes a block of code if a given condition is true. Example:</li></ul><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">if</span> (age &gt; <span class="hljs-number">18</span>) {
    <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-string">"You are an adult."</span>);
}
</code></div></div></pre><ul><li>else: Executes a block of code if the preceding if statement's condition is false. Example:</li></ul><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">if</span> (age &gt; <span class="hljs-number">18</span>) {
    <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-string">"You are an adult."</span>);
} <span class="hljs-keyword">else</span> {
    <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-string">"You are not an adult."</span>);
}
</code></div></div></pre><ul><li>else if: Used in conjunction with if and else to test multiple conditions. Example:</li></ul><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">if</span> (age &lt; <span class="hljs-number">18</span>) {
    <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-string">"You are a minor."</span>);
} <span class="hljs-keyword">else</span> <span class="hljs-keyword">if</span> (age &gt;= <span class="hljs-number">18</span> &amp;&amp; age &lt; <span class="hljs-number">65</span>) {
    <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-string">"You are an adult."</span>);
} <span class="hljs-keyword">else</span> {
    <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-string">"You are a senior."</span>);
}
</code></div></div></pre></li><li>Loops:<ul><li>for: Executes a block of code a certain number of times. Example:</li></ul><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-css">for (let <span class="hljs-selector-tag">i</span> = <span class="hljs-number">0</span>; <span class="hljs-selector-tag">i</span> &lt; <span class="hljs-number">5</span>; <span class="hljs-selector-tag">i</span>++) {
    console<span class="hljs-selector-class">.log</span>(<span class="hljs-selector-tag">i</span>);
}
// Output: <span class="hljs-number">0</span> <span class="hljs-number">1</span> <span class="hljs-number">2</span> <span class="hljs-number">3</span> <span class="hljs-number">4</span>
</code></div></div></pre><ul><li>while: Executes a block of code while a given condition is true. Example:</li></ul><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">let</span> i = <span class="hljs-number">0</span>;
<span class="hljs-keyword">while</span> (i &lt; <span class="hljs-number">5</span>) {
    <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(i);
    i++;
}
<span class="hljs-comment">// Output: 0 1 2 3 4</span>
</code></div></div></pre><ul><li>do-while: Similar to while, but the block of code is executed at least once. Example:</li></ul><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">let</span> i = <span class="hljs-number">0</span>;
<span class="hljs-keyword">do</span> {
    <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(i);
    i++;
} <span class="hljs-keyword">while</span> (i &lt; <span class="hljs-number">5</span>);
<span class="hljs-comment">// Output: 0 1 2 3 4</span>
</code></div></div></pre></li><li>switch-case: Used to perform different actions based on different conditions. Example:</li></ul><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">let</span> day = <span class="hljs-string">"Monday"</span>;
<span class="hljs-keyword">switch</span> (day) {
    <span class="hljs-keyword">case</span> <span class="hljs-string">"Monday"</span>:
        <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-string">"It's Monday."</span>);
        <span class="hljs-keyword">break</span>;
    <span class="hljs-keyword">case</span> <span class="hljs-string">"Tuesday"</span>:
        <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-string">"It's Tuesday."</span>);
        <span class="hljs-keyword">break</span>;
    <span class="hljs-keyword">case</span> <span class="hljs-string">"Wednesday"</span>:
        <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-string">"It's Wednesday."</span>);
        <span class="hljs-keyword">break</span>;
    <span class="hljs-attr">default</span>:
        <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-string">"It's another day."</span>);
}
<span class="hljs-comment">// Output: "It's Monday."</span>
</code></div></div></pre></li></ol><p>It's worth noting that the default statement is optional, but it's a good practice to include it as it helps to handle unexpected cases.
Also, switch-case statements are more efficient than a series of if-else statements when testing for multiple conditions, especially when the conditions are string literals.</p></div>
