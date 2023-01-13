<div class="markdown prose w-full break-words dark:prose-invert light"><p>Examples to help explain variable scope in JavaScript:</p><ol><li>Global scope: Variables declared outside of any function or block have global scope. They can be accessed and modified from anywhere in the code.</li></ol><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">let</span> name = <span class="hljs-string">"John"</span>;

<span class="hljs-keyword">function</span> <span class="hljs-title function_">printName</span>(<span class="hljs-params"></span>) {
<span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(name); <span class="hljs-comment">// Output: "John"</span>
}
</code></div></div></pre><ol start="2"><li>Local scope: Variables declared within a function or block have local scope and can only be accessed within that function or block.</li></ol><pre><div class="bg-black mb-4 rounded-md"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-scss">function <span class="hljs-built_in">printAge</span>() {
let age = <span class="hljs-number">25</span>;
console<span class="hljs-selector-class">.log</span>(age); <span class="hljs-comment">// Output: 25</span>
}
<span class="hljs-built_in">printAge</span>();
console<span class="hljs-selector-class">.log</span>(age); <span class="hljs-comment">// ReferenceError: age is not defined</span>
</code></div></div></pre><ol start="3"><li>Block scope: Variables declared with <code>let</code> or <code>const</code> within a block (e.g. a set of curly braces <code>{}</code>) have block scope and can only be accessed within that block.</li></ol><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">if</span> (<span class="hljs-literal">true</span>) {
<span class="hljs-keyword">let</span> message = <span class="hljs-string">"Hello!"</span>;
<span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(message); <span class="hljs-comment">// Output: "Hello!"</span>
}
<span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(message); <span class="hljs-comment">// ReferenceError: message is not defined</span>
</code></div></div></pre><ol start="4"><li>Function scope: Variables declared within a function have function scope and can be accessed within that function, but not outside it.</li></ol><pre><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-scss">function <span class="hljs-built_in">showResult</span>() {
<span class="hljs-selector-tag">var</span> score = <span class="hljs-number">85</span>;
console<span class="hljs-selector-class">.log</span>(score); <span class="hljs-comment">// Output: 85</span>
}
<span class="hljs-built_in">showResult</span>();
console<span class="hljs-selector-class">.log</span>(score); <span class="hljs-comment">// ReferenceError: score is not defined</span>
</code></div></div></pre><p>It's important to note that <code>var</code> keyword variables in JavaScript are function scoped, meaning they are only accessible within the function they were declared in, while <code>let</code> and <code>const</code> are block scoped, meaning they are only accessible within the block they were declared in.</p><p>It's also worth noting that variables declared with <code>var</code> are hoisted to the top of their scope, meaning they can be accessed before they are declared, while variables declared with <code>let</code> and <code>const</code> are not hoisted, and will result in a ReferenceError if accessed before they are declared.</p></div>
