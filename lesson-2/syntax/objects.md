<div class="markdown prose w-full break-words dark:prose-invert dark"><p>Sure, here's more information on objects in JavaScript, along with examples of how to use them:</p><ol start="7"><li>Objects<ul><li>Understanding object literals:</li></ul><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">let</span> person = {
    <span class="hljs-attr">name</span>: <span class="hljs-string">"John"</span>,
    <span class="hljs-attr">age</span>: <span class="hljs-number">30</span>,
    <span class="hljs-attr">isStudent</span>: <span class="hljs-literal">false</span>
};
<span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(person.<span class="hljs-property">name</span>); <span class="hljs-comment">// Output: "John"</span>
<span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(person[<span class="hljs-string">"age"</span>]); <span class="hljs-comment">// Output: 30</span>
</code></div></div></pre><ul><li>Creating objects using constructors:</li></ul><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">function</span> <span class="hljs-title function_">Person</span>(<span class="hljs-params">name, age, isStudent</span>) {
    <span class="hljs-variable language_">this</span>.<span class="hljs-property">name</span> = name;
    <span class="hljs-variable language_">this</span>.<span class="hljs-property">age</span> = age;
    <span class="hljs-variable language_">this</span>.<span class="hljs-property">isStudent</span> = isStudent;
}
<span class="hljs-keyword">let</span> john = <span class="hljs-keyword">new</span> <span class="hljs-title class_">Person</span>(<span class="hljs-string">"John"</span>, <span class="hljs-number">30</span>, <span class="hljs-literal">false</span>);
<span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(john.<span class="hljs-property">name</span>); <span class="hljs-comment">// Output: "John"</span>
</code></div></div></pre><ul><li>Adding and removing properties from objects:</li></ul><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-css">let car = {
    make: <span class="hljs-string">"Honda"</span>,
    model: <span class="hljs-string">"Civic"</span>
};
car<span class="hljs-selector-class">.year</span> = <span class="hljs-number">2020</span>; // Adding property
console<span class="hljs-selector-class">.log</span>(car); // Output: { make: <span class="hljs-string">'Honda'</span>, model: <span class="hljs-string">'Civic'</span>, year: <span class="hljs-number">2020</span> }
delete car<span class="hljs-selector-class">.year</span>; // Removing property
console<span class="hljs-selector-class">.log</span>(car); // Output: { make: <span class="hljs-string">'Honda'</span>, model: <span class="hljs-string">'Civic'</span> }
</code></div></div></pre><ul><li>Understanding the prototype chain:</li></ul><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">function</span> <span class="hljs-title function_">Person</span>(<span class="hljs-params">name</span>) {
    <span class="hljs-variable language_">this</span>.<span class="hljs-property">name</span> = name;
}
<span class="hljs-title class_">Person</span>.<span class="hljs-property"><span class="hljs-keyword">prototype</span></span>.<span class="hljs-property">sayHello</span> = <span class="hljs-keyword">function</span>(<span class="hljs-params"></span>) {
    <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-string">"Hello, my name is "</span> + <span class="hljs-variable language_">this</span>.<span class="hljs-property">name</span>);
}
<span class="hljs-keyword">let</span> john = <span class="hljs-keyword">new</span> <span class="hljs-title class_">Person</span>(<span class="hljs-string">"John"</span>);
john.<span class="hljs-title function_">sayHello</span>(); <span class="hljs-comment">// Output: "Hello, my name is John"</span>
</code></div></div></pre></li></ol><p>It's worth noting that object literals are a shorthand way to create objects and are useful for creating small, simple objects.
Object constructors are a way to create objects with a specific structure, and are useful for creating multiple objects with the same structure.</p><p>Also, in JavaScript, all objects have a prototype, which is an object that provides shared properties and methods. The prototype is used to implement inheritance and polymorphism in the language.</p></div>