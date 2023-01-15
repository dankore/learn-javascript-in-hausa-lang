<div><p>Examples of variable declaration and assignment in JavaScript:</p><ol><li>Variable declaration using the <code>var</code> keyword:</li></ol><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">var</span> name = <span class="hljs-string">"John"</span>;
<span class="hljs-keyword">var</span> age = <span class="hljs-number">30</span>;
<span class="hljs-keyword">var</span> isStudent = <span class="hljs-literal">true</span>;
</code></div></div></pre><ol start="2"><li>Variable declaration using the <code>let</code> keyword:</li></ol><pre><div class="bg-black mb-4 rounded-md"><div class="flex items-center relative text-gray-200 bg-gray-800 px-4 py-2 text-xs font-sans"></div><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">let</span> city = <span class="hljs-string">"New York"</span>;
<span class="hljs-keyword">let</span> country = <span class="hljs-string">"United States"</span>;
<span class="hljs-keyword">let</span> population = <span class="hljs-number">8000000</span>;
</code></div></div></pre><ol start="3"><li>Variable declaration using the <code>const</code> keyword:</li></ol><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">const</span> <span class="hljs-variable constant_">PI</span> = <span class="hljs-number">3.14</span>;
<span class="hljs-keyword">const</span> gravity = <span class="hljs-number">9.8</span>;
<span class="hljs-keyword">const</span> <span class="hljs-variable constant_">MAX_SPEED</span> = <span class="hljs-number">300</span>;
</code></div></div></pre><ol start="4"><li>Reassign the value of variable using the assignment operator (=):</li></ol><pre><div class="bg-black mb-4 rounded-md"><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">let</span> numberOfStudents = <span class="hljs-number">25</span>;
numberOfStudents = <span class="hljs-number">30</span>; 
<span class="hljs-variable language_">console</span>.<span class="hljs-title function_">log</span>(numberOfStudents); <span class="hljs-comment">// Output: 30</span>
</code></div></div></pre><ol start="5"><li>declare and assign multiple variables in one line:</li></ol><pre><div class="p-4 overflow-y-auto"><code class="!whitespace-pre-wrap hljs language-javascript"><span class="hljs-keyword">let</span> x = <span class="hljs-number">1</span>, y = <span class="hljs-number">2</span>, z = <span class="hljs-number">3</span>;
<span class="hljs-keyword">let</span> a = <span class="hljs-number">4</span>, b = <span class="hljs-number">5</span>, c = <span class="hljs-number">6</span>;
</code></div></div></pre><p>It's important to note that variables declared using the <code>const</code> keyword cannot be reassigned. Attempting to do so will result in a TypeError. Also, it's recommended to use <code>let</code> or <code>const</code> instead of <code>var</code> when declaring variables, as <code>var</code> has some unexpected behavior in certain cases.</p></div>