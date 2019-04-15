# CUNY Student Editions CSS Style Sheet
<h1 id="top">Table of Contents</h1>
<ul>
	<li><a href="#how-to-use">1.0 How to Use this Style Sheet</a></li>
	<li><a href="#pages-sections">2.0 Pages/Sections</a></li>
		<ul>
			<li><a href="#basic-structure">2.1 Basic Page Structure</a></li>
			<li><a href="#title-page">2.2 Title Page</a></li>
			<li><a href="#copyright-page">2.3 Copyright Page</a></li>
		</ul>
	<li><a href="#formatting">3.0 Formatting Text</a></li>
		<ul>
			<li><a href="#ct>3.1 Chapter title</a></li>
			<li><a href="#pf">3.2 Chapter's first paragraph</a></li>
			<li><a href="#attribution">3.3 Attribution</a></li>
			<li><a href="#quote">3.4 Block quotes</a></li>
			<li><a href="#poetry">3.5 Poetry/epigraph</a></li>
			<li><a href="#footnotes">3.6 Footnotes</a></li>
			<li><a href="#all-else">3.7 When All Else Fails</a> (individual text formatting elements)</li>
		</ul>
	<li><a href="#images">3.0 Images</li>
	<li><a href="#organized">4.0 How the Style Sheet is Organized</a></li>
</ul>
<p><a href="#top">(Back to Top)</a></p>
<hr/>
	
<h1 id="how-to-use">1.0 How to Use this Style Sheet</h1>
<p>This is the default CSS style sheet used to create CUNY Student Editions. It is the code version of of our house styles, giving CUNY Student Editions their unique look and feel. It is desigend to give consistancy across ereaders, including CUNY Manifold where all CUNY Student Editions are published.</p>
<p>This sytle sheet is offered to the public at no cost under a Creative Commons <a href="https://creativecommons.org/licenses/by/4.0/" target=”_blank”>Attribution 4.0 International License</a>. You are free to share, remix or reuse it anyway to digitize your own texs.</p>
<p>In return, all we ask is that you please include a shout out to CUNY Student Editions and our GitHub site (https://github.com/CUNY-Student-Editions)in your code or text.</p>
<p><a href="#top">(Back to Top)</a></p>
<hr/>
  
<h1 id="pages-sections">2.0 Pages/Sections</h1>
<p>More soon.</p>
<p><a href="#top">(Back to Top)</a></p>

<h2 id="basic-structure">2.1 Basic Page Structure</h2>
<p>Each .html page in the book should open and close with a <b>body</b> .div tag.</p>
<p>Example:</p>
<p><pre><code>&lt;body&gt;</br/>
&lt;/body&gt;</code></pre></p>
<p>This <b>body</b> tag applies the most basic styles to the page such <code>page-width, font, font-size,</code> etc. It also prevents errors with certain e-readers that require all elements to be wrapped in a div tag.</p>
<p>Most .html pages will then be further styled with a <b>chapter</b> or <b>section</b> .div tag.</p>
<p><i>Example</i><br/>
<pre><code>&lt;body&gt;<br/>
&lt;div class="chapter"&gt;<br/>
&lt;p&gt;This is the text of your chapter&lt;/p&gt;<br/>
&lt;/div&gt;<br/>
&lt;/body&gt;</code></pre></p>
<p>You can have multiple sections or chapters on a single .html page as well as nested inside each other.</p>
<p><i>Example</i><br/>
<pre><code>&lt;body&gt;<br/>
&lt;div class="chapter"&gt;<br/>
&lt;div class="section"&gt;<br/>
&lt;p&gt;This is the text of your chapter's first section.&lt;/p&gt;<br/>
&lt;/div&gt;<br/>
&lt;div class="section"&gt;<br/>
&lt;p&gt;This is the text of your chapter's second section.&lt;/p&gt;<br/>
&lt;/div&gt;<br/>
&lt;/div&gt;<br/>
&lt;/body&gt;</code></pre></p>
<p><b>Chapters</b> and <b>sections</b> are formatted similarly but have different endspacing.</p>
<p><b>Chapters</b> have four lines (4em) of end space.</p>
<p><b>Sections</b> have three lines (3em) of endspace.</p>
<p><a href="#top">(Back to Top)</a></p>

<h2 id="title-page">2.2 Title Page</h2>
<p>Title pages are uniquely styled and so do not require a <b>chapter</b> or <b>section</b> .div tag. Instead, the <b>body</b>tag is sufficient. Instead, elements are styled according to the information hierarchy.</p>
<ul>
	<li>h1 = Title</li>
	<li>h2 = Subtitles</li>
	<li>h3 = Author, Editor</li>
	<li>p = Editor's Affiliation, CUNY Student Edition Banner, anything else</li>
	</ul>
<p><i>Example</i></p>
<p><pre><code>&lt;h1 class="title"&gt;Adventures of Huckleberry Finn&lt;/h1&gt;<br/>
&lt;h2 class="subtitle"&gt;(Tom Sawyer's Comrade)&lt;/h2&gt;<br/>
&lt;h2 class="subtitle2"&gt;Scene: The Mississippi Valley&lt;br/&gt;<br/>
Time: Forty to Fifty Years Ago&lt;/h2&gt;<br/>
&lt;h3 class="author"&gt;Mark Twain&lt;/h3&gt;<br/>
&lt;h3 class="editor"&gt;Edited by Paul L. Hebert&lt;/h3&gt;<br/>
&lt;p class="ed2"&gt;City University of New York&lt;/p&gt;<br/>
&lt;p class="banner"&gt;CUNY Student Edition&lt;/p&gt;</code></pre></p>
<p><a href="#top">(Back to Top)</a></p>

<h2 id="copyright-page">2.3 Copyright Page</h2>
<p>CUNY Student Editions are not copyrighted and so do not include this page. Instead, the license information is included in a Note about the Text. Styles for a copyright pages are included here, however, to assist others.</p>
<p>Copyright pages have unique formatting and so use the <b>copyright</b> .div tag instead of the chapter/section .div tags.</p>
<p>There are no headings for the copright pages, only <b>paragraph</b> tags.</p>
<p><i>Example</i></p>
<p><pre><code>&lt;body&gt;<br/>
 &lt;div class="copyright"&gt;<br/>
&lt;p&gt;First Published in Boston: For the Author [Harriet Ann Jacobs], 1861.&lt;/p&gt;<br/>
&lt;p&gt;Last updated 7 Nov. 2018&&lt;/p&gt;<br/>
&lt;p&gt;This work is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License:&lt;br/&gt;<br/>
http://creativecommons.org/licenses/by-sa/4.0/&lt;p&gt<br/>
&lt;p&gt;Cover Photograph: "Portrait of Harriet Jacobs". &lt;span class="it"&gt;Documenting the American South&lt;/span&gt;.<br/> University Library, The University of North Carolina at Chapel Hill. 7 January 2004.<br/> https://docsouth.unc.edu/fpn/jacobs/jacobs_100.html&lt;/p&gt;<br/>
&lt;p&gt;Edited and published by Paul L. Hebert,&lt;br/&gt;<br/>
City University of New York (CUNY)</p&gt;<br/>
&lt;/div&gt;</br>
	&lt;/body&gt;</code></pre></p>

<p><a href="#top">(Back to Top)</a></p>	
<hr/>

<h1 id="formatting">3.0 Formatting Text</h1>
<p>All text formatting should be done with CSS styles rather than HTML elements. For example, use <code>&lt;span class=".it"&gt;</code> to format a word in italics rather than <code>&lt;i&gt;</code>. This increases consistancy across e-readers and makes some changes to ebooks easier.</p>
<p>Similar to <a href="https://tei-c.org/" target="_blank">TEI encoding, the code of a text should help someone understand the structure of the page. That's why it's prefarable to style a stanza of poetry with a 
<p><a href="#top">(Back to Top)</a></p>	

<h2 id="ct">3.1 Chapter Title</h2>
<p>The title of a chapter or section has unique styling. Use <code>&lt;h1 class="ct"&gt;</code> (for "chapter title").</p>
<p><a href="#top">(Back to Top)</a></p>	

<h2 id="pf">3.2 First Paragraph of a Chapter</h2>
<p>The first paragraph in a chapter or section has unique styling to differentiate it from other text. Therefore, the first paragraph in a chapter should use the <code>&lt;p class="pf"&gt;</code> (for "Paragraph, first").</p>
<p><a href="#top">(Back to Top)</a></p>	

<h2 id="attribution">3.3. Attribution</h2>
<p>More soon.</p>
<p><a href="#top">(Back to Top)</a></p>	

<h2 id-"quote">3.4 Block Quotes</h2>
<p>More soon.</p>
<p><a href="#top">(Back to Top)</a></p>	
			
<h2 id="poetry">3.5 Poetry/Epigraphs</h2>
<p>More soon.</p>
<p>Organized by class="stanza", includes hanging indent for fluid text. 
<p><a href="#top">(Back to Top)</a></p>	

<h2 id="footnotes">3.6 Footnotes</h2>
<p>CUNY Student Editions are designed as fluid texts, meaning that the layout of the page is mostly determined by a particular ereader. As a result, footnotes function more like endnotes, appearing at the bottom of the end of the section, chpater, or .html page.</p>
<p>To create a footnote:</p>
<ol>
	<li>Insert a numeral/letter in the text to indicate a footnote.</li>
	<li>Style the numeral as superscript.</li>
	<li>At the bottom of the section/chapter/page, insert the Footnotes Wrapper to create a horizontal rule and style the footnotes</li>
	<li>Type your footnote.</li>
	<li>Link your footnotes with an in-page hyperlink.</li>
	</ol>
<p><i>Example</i>
<pre><code>&lt;body&gt;<br/>
&lt;div class="chapter"&gt;<br/>
&lt;p&gt;This is the text of your chapter&lt;span class="sup" id="cite-1"&gt;&lt;a href="#note-1"&gt;1&lt;/class&gt;&lt;/a&gt;&lt;/p&gt;<br/>
&lt;div class="footnotes"&gt;<br/>
&lt;p id="note-1"&gt;&lt;a href="#cite-1"&gt;[1]&lt;/a&gt; This is your note.&lt;/p&gt;<br/>
&lt;/div&gt;<br/>
&lt;/div&gt;<br/>
&lt;/body&gt;</code></pre></p>
<p><a href="#top">(Back to Top)</a></p>	

<h2 id="all-else">3.7 Everything Else</h2>
<p>These should be used sparingly, but help when you just can't get anything else to work or when the formatting is used only in a few instances.</p>
<ul>
	<li>Alignment</li>
		<ul>
			<li>Center ("center")</li>
			<li>Right justified ("rt")</li>
		</ul>
	<li>Supepscript/subscript</li>
		<ul>
			<li>Superscript ("sup")</li>
		</ul>
	<li>Font Style</li>
		<ul>
			<li><i>Italics</i> ("it")</li>
			<li><b>Bold</b> ("bld")</li>
			<li>SMALL CAPS ("sc")</li>
		</ul>
	</ul>
<p><a href="#top">(Back to Top)</a></p>	

<h1 id="images">4.0 Images</a></h1>
<p>More soon.</p>
<p><a href="#top">(Back to Top)</a></p>

<h1 id="organized">5.0 How the Style Sheet is Organized</a></h1>
  	<ul>
  		<li>Manifold Style</li>
  		<li>CUNY Student Edition - House Styles</li>
				<ul>
					<li>Basic Elements</li>
      			<ul>
        			<li>Headings (H1, H2, H3)</li>
        			<li>Horizontal rule (hr)</li>
							<li>imgages</li>
      			  </ul>
      			<li>Text formating</li>
        			<ul>
          			<li>Text alignment (center, right)</li>
          			<li>Font style (bold, italic)</li>
          			<li>Font variant (small caps)</li>
      					</ul>
					<li>Title page elements/sytles</li>
					<li>Copyright page styles</li>
					<li>Chapter/Section styles</li>
					<li>Special paragraph styles</li>
						<ul>
							<li>Poetry/Epigraph</li>
							<li>Footnotes</li>
							<li>Attribution</li>
						</ul>
  				</ul>
    		</ul>
<p><a href="#top">(Back to Top)</a></p>				
<hr/>
  

