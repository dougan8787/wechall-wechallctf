<h2>Training: Get Sourced</h2>
 <pre><code>Look Sourcecode get password:html_sourcecode</code></pre>
 
<h2>Training: Stegano I</h2>
<pre><code>TextEd Look Stegano I.bmp get passwd:steganoI</code></pre>

<h2>Training: WWW-Robots</h2>
<pre><code>www.wechall.net/robots.txt</code></pre>

<h2>Training: ASCII</h2>
<pre><code>Decimal (84, 104, 101, 32, 115, 111, 108, 117, 116, 105, 111, 110, 32, 105, 115, 58, 32, 115, 109, 104, 110, 102, 109, 97, 101, 109, 100, 100, 105) decode Ascii code</code></pre>

<h2>Encodings: URL</h2>
<pre><code>URL (%59%69%70%70%65%68%21%20%59%6F%75%72%20%55%52%4C%20%69%73%20%63%68%61%6C%6C%65%6E%67%65%2F%74%72%61%69%6E%69%6E%67%2F%65%6E%63%6F%64%69%6E%67%73%2F%75%72%6C%2F%73%61%77%5F%6C%6F%74%69%6F%6E%2E%70%68%70%3F%70%3D%6E%6E%68%61%63%65%65%6D%6F%6F%6C%63%26%63%69%64%3D%35%32%23%70%61%73%73%77%6F%72%64%3D%66%69%62%72%65%5F%6F%70%74%69%63%73%20%56%65%72%79%20%77%65%6C%6C%20%64%6F%6E%65%21) decode to ascii (Yippeh! Your URL is challenge/training/encodings/url/saw_lotion.php?p=nnhaceemoolc&cid=52#password=fibre_optics Very well done! ) change url</code></pre>

<h2>Training: PHP LFI</h2>
<pre><code>PHP code
$filename = 'pages/'.(isset($_GET["file"])?$_GET["file"]:"welcome").'.html';
include $filename;
</code><pre>
<h3>把原本index.php?file=new先改成?file=solution.php得知路徑不同，加上../../solution.php，結果報錯是因為後面有.html的格式加進來變成../../solution.php.html為了防止它加進來後面加上%00空字符</h3>

