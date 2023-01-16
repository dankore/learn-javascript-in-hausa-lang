- [Simple program in JavaScript](#Simple-program-in-JavaScript)
- [Using the JavaScript console to run and debug code](#Using-the-JavaScript-console-to-run-and-debug-code)
- [Basic error handling in JavaScript](#Basic-error-handling-in-JavaScript)
- [Working with strings and numbers in JavaScript](#Working-with-strings-and-numbers-in-JavaScript)

<div class="markdown prose w-full break-words dark:prose-invert dark"><p id="Simple-program-in-JavaScript">Simple program in JavaScript that prints "Hello, World!" to the console:</p><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(<span class="hljs-string">"Hello, World!"</span>);
</code></div></div></pre><p>You can run this program by opening the JavaScript console in your browser (usually by pressing F12 or right-clicking and selecting "Inspect Element" and then selecting the "Console" tab), and pasting the above code into the console and pressing enter.</p><p>You can also use Node.js to run JavaScript code outside of a web browser.</p><p>In order to write and run JavaScript code, you will need a text editor, such as Notepad, Sublime Text, or Visual Studio Code, and a web browser or Node.js environment.</p><p>You can also use the JavaScript console to debug your code by adding the following line before the <code>console.log</code> statement</p><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span id="Using-the-JavaScript-console-to-run-and-debug-code" class="hljs-keyword">debugger</span>;
</code></div></div></pre><p id="Basic-error-handling-in-JavaScript">Here is an example of basic error handling in JavaScript:</p><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">try</span> {
  <span class="hljs-comment">// code that may throw an error</span>
  <span class="hljs-keyword">let</span> x = y; <span class="hljs-comment">// y is not defined</span>
} <span class="hljs-keyword">catch</span> (error) {
  <span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(error); <span class="hljs-comment">// Output: ReferenceError: y is not defined</span>
}
</code></div></div></pre><p id="Working-with-strings-and-numbers-in-JavaScript">And here is an example of working with strings and numbers in JavaScript:</p><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">let</span> firstName = <span class="hljs-string">"John"</span>;
<span class="hljs-keyword">let</span> lastName = <span class="hljs-string">"Doe"</span>;
<span class="hljs-keyword">let</span> fullName = firstName + <span class="hljs-string">" "</span> + lastName;
<span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(fullName); <span class="hljs-comment">// Output: "John Doe"</span>

<span class="hljs-keyword">let</span> a = <span class="hljs-number">10</span>;
<span class="hljs-keyword">let</span> b = <span class="hljs-number">20</span>;
<span class="hljs-keyword">let</span> sum = a + b;
<span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(sum); <span class="hljs-comment">// Output: 30</span>
</code></div></div></pre></div>
