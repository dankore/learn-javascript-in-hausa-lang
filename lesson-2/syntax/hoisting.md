<div class="markdown prose w-full break-words dark:prose-invert light"><p>Examples that demonstrate hoisting in JavaScript:</p><ol><li>Variable hoisting with <code>var</code>:</li></ol><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(x); <span class="hljs-comment">// undefined</span>
<span class="hljs-keyword">var</span> x = <span class="hljs-number">5</span>;
<span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(x); <span class="hljs-comment">// 5</span>
</code></div></div></pre><p>In this example, the variable <code>x</code> is declared with the <code>var</code> keyword and is initialized with the value <code>5</code>. The first <code>console.log()</code> statement outputs <code>undefined</code> because variable hoisting moves the variable declaration to the top of the scope, but not the assignment, so the variable is undefined at that point. The second <code>console.log()</code> statement outputs <code>5</code>, as the variable has been assigned the value of <code>5</code>.</p><ol start="2"><li>Variable hoisting with <code>let</code>:</li></ol><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(x); <span class="hljs-comment">// ReferenceError: x is not defined</span>
<span class="hljs-keyword">let</span> x = <span class="hljs-number">5</span>;
<span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(x);
</code></div></div></pre><p>In this example, the variable <code>x</code> is declared with the <code>let</code> keyword and is initialized with the value <code>5</code>. The first <code>console.log()</code> statement throws a <code>ReferenceError</code> because variable hoisting is not applied to variables declared with <code>let</code> or <code>const</code>, and the variable is not defined at that point.</p><ol start="3"><li>Function hoisting:</li></ol><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-scss"><span class="hljs-built_in">hoisted</span>(); <span class="hljs-comment">// "I'm a hoisted function!"</span>

function <span class="hljs-built_in">hoisted</span>() {
  console<span class="hljs-selector-class">.log</span>("I'm a hoisted function!");
}

<span class="hljs-built_in">notHoisted</span>(); <span class="hljs-comment">// ReferenceError: notHoisted is not a function</span>

let notHoisted = <span class="hljs-built_in">function</span>() {
  console<span class="hljs-selector-class">.log</span>("I'm not a hoisted function!");
}
</code></div></div></pre><p>In this example, the function <code>hoisted</code> is hoisted to the top of the scope, so it can be called before it is defined. However, the function <code>notHoisted</code> declared with the <code>let</code> keyword is not hoisted, and thus it throws a <code>ReferenceError</code> when called before it is defined.</p><p>It's important to note that hoisting is a behavior specific to variable and function declarations, not variable assignments.</p></div>