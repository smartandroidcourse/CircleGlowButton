<ol dir="auto">
<li>
<p dir="auto">Include the library as local library project:</p>
<div class="highlight highlight-source-groovy notranslate position-relative overflow-auto" dir="auto">
<pre><code id="depCodeGradle" class=" kode  language-css">maven <span class="token string">{url 'https://jitpack.io'}</span></code><span class="pl-s"><span class="pl-pds"><br /><br /></span></span></pre>
</div>
</li>
<li>
<p dir="auto">Include the library as local library project:</p>
<div class="highlight highlight-source-groovy notranslate position-relative overflow-auto" dir="auto">
<pre><code id="depCodeGradle" class=" kode  language-css">implementation <span class="token string">'com.github.smartandroidcourse:CircleGlowButton:1.0</span></code><span class="pl-s"><span class="pl-pds">'<br /><br /></span></span></pre>
</div>
</li>
<li>
<p dir="auto">Add view to your layout file:</p>
<div class="highlight highlight-text-xml notranslate position-relative overflow-auto" dir="auto">
<pre><span class="pl-c"><span class="pl-c">&lt;!--</span> ... <span class="pl-c">--&gt;</span></span></pre>
<pre>&lt;colorsfx.smart.android.courses.circleglowbutton.CircleGlow<br />    android:id="@+id/btnClick"<br />    android:layout_width="120dip"<br />    android:layout_height="120dip"<br />    android:src="@drawable/ic_launcher_foreground"<br />    android:layout_centerInParent="true"<br />    app:cb_color="#29AC05"<br />    app:cb_pressedRingWidth="8dip" /&gt;</pre>
<pre><span class="pl-c"><span class="pl-c">&lt;!--</span> ... <span class="pl-c">--&gt;</span></span></pre>
<div class="zeroclipboard-container position-absolute right-0 top-0">&nbsp;</div>
</div>
</li>
<li>
<p dir="auto">Add component handler into your activity or fragment (Java):</p>
<div class="highlight highlight-source-java notranslate position-relative overflow-auto" dir="auto">
<pre>CircleGlow btnClick = findViewById(R.id.btnClick);<br /><br />btnClick.setOnClickListener(new View.OnClickListener() {<br />@Override<br />public void onClick(View v) {<br /><br />Toast.makeText(getApplicationContext(),"Clicked",Toast.LENGTH_SHORT).show();<br /><br />}<br />});</pre>
<div class="zeroclipboard-container position-absolute right-0 top-0">&nbsp;</div>
</div>
</li>
<li>
<p dir="auto">Add component handler into your activity or fragment (Kotlin):</p>
<div class="highlight highlight-source-java notranslate position-relative overflow-auto" dir="auto">
<pre>lateinit var btnClick : CircleGlow </pre>
<pre>btnClick.setOnClickListener(View.OnClickListener {<br />    Toast.makeText(<br />        applicationContext,<br />        "Clicked",<br />        Toast.LENGTH_SHORT<br />    ).show()<br />})</pre>
<div class="zeroclipboard-container position-absolute right-0 top-0">&nbsp;</div>
</div>
</li>
</ol>
