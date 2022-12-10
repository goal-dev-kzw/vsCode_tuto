## VSCode Emmet Abbreviation

***Write Code More Easily & Quickly***

🔴 <mark><u><b>*Tag*</b></u></mark>

     1️⃣ h1
    -------------------------------------------------------------------------------------------------------------------------------
     1️⃣  <h1></h1>

<br>

🔴 <mark><u><b>*Text*</b></u></mark>

  

     1️⃣ h1{Hello World}
     2️⃣ a{Click me}
    -------------------------------------------------------------------------------------------------------------------------------
     1️⃣ <h1>Hello World</h1>
     2️⃣ <a href="">Click me</a>

<br>

🔴 <mark><u><b>*id | class*</b></u></mark>


    1️⃣ #header
    2️⃣ .title
    3️⃣ form#search.wide
    4️⃣ p.class1.class2.class3
    -------------------------------------------------------------------------------------------------------------------------------
    1️⃣ <div id="header"></div>
    2️⃣ <div class="title"></div>
    3️⃣ <form id="search" class="wide"></form>
    4️⃣	<p class="class1 class2 class3"></p>

<br>

🔴 <mark><u><b>*Attributes*</b></u></mark>


    1️⃣ p[title="Hello world"]
    2️⃣ td[rowspan=2 colspan=3 title
    -------------------------------------------------------------------------------------------------------------------------------
    1️⃣ <p title="Hello world"></p>
    2️⃣ <td rowspan="2" colspan="3" title=""></td>
   
<br>


🔴 <mark><u><b>*Child Tags*</b></u></mark>


    1️⃣ nav>ul>li
    2️⃣ div>h5{Hello}
    -------------------------------------------------------------------------------------------------------------------------------
    1️⃣ <nav> 
		  <ul> 
		    <li></li> 
		  </ul> 
		</nav>
		
    2️⃣ <div>
		  <h5>Hello</h5>
	   </div>
   
<br>


🔴 <mark><u><b>*Siblings*</b></u></mark>


    1️⃣ div+p+bq
    2️⃣ h3+p+span
    -------------------------------------------------------------------------------------------------------------------------------
    1️⃣ <div></div> 
	   <p></p> 
	   <blockquote></blockquote>
		
    2️⃣ <h3></h3>
	    <p></p>
	    <span></span>
   
<br>


🔴 <mark><u><b>*Climb-up*</b></u></mark>


    1️⃣ div+div>p>span+em^bq
    2️⃣ div+div>p>span+em^^bq
    -------------------------------------------------------------------------------------------------------------------------------
    1️⃣ <div></div> 
	   <div> 
		  <p> <span></span><em></em> </p>
	      <blockquote></blockquote>
	   </div>
		
    2️⃣ <div></div> 
       <div> <p><span></span><em></em></p> </div> 
       <blockquote></blockquote>
   

<br>


🔴 <mark><u><b>*Multiple Tags*</b></u></mark>


    1️⃣ h1*3
    2️⃣ ul>li*5
    -------------------------------------------------------------------------------------------------------------------------------
    1️⃣ <h1></h1>
	   <h1></h1>
       <h1></h1>
       
    2️⃣ <ul> 
	     <li></li>
	     <li></li>
	     <li></li>
	     <li></li> 
	     <li></li> 
       </ul>

<br>

🔴 <mark><u><b>*Item Numbering*</b></u></mark>


    1️⃣ p{Hello $}*3
    2️⃣ p{Hello $$$}*3
    3️⃣ ul>li.item$*5{$$ Item}
    4️⃣ h${Header $}*3
    -------------------------------------------------------------------------------------------------------------------------------
    1️⃣ <p>Hello 1</p>
	   <p>Hello 2</p>
	   <p>Hello 3</p>

    2️⃣ <p>Hello 001</p>
	   <p>Hello 002</p>
	   <p>Hello 003</p>

    3️⃣ <ul>
	      <li class="item1">01 Item</li> 
	      <li class="item2">02 Item</li>
	      <li class="item3">03 Item</li>
	      <li class="item4">04 Item</li> 
	      <li class="item5">05 Item</li> 
       </ul>
       
    4️⃣	<h1>Header 1</h1>
		<h2>Header 2</h2>
		<h3>Header 3</h3>


<br>


🔴 <mark><u><b>*Groupings*</b></u></mark>


    1️⃣ div>(header>ul>li*2>a)+footer>p
    -------------------------------------------------------------------------------------------------------------------------------
    1️⃣ <div> 
	      <header> 
	        <ul> 
			    <li><a href=""></a></li>
			    <li><a href=""></a></li> 
		    </ul> 
	      </header> 
	      <footer> 
	           <p></p> 
	     </footer> 
	   </div>
       
 


    

<br>


🔴 <mark><u><b>*Pratice Example*</b></u></mark>


     <div>    
	    <header>    
		    <h2>Header 01</h2>    
		    <h2>Header 02</h2>    
		    <h2>Header 03</h2>    
		    <p>This is a paragraph.</p>    
		    <ul  class="nav">    
			    <li  id="list1">List 001</li>    
			    <li  id="list2">List 002</li>    
			    <li  id="list3">List 003</li>    
			    <li  id="list4">List 004</li>    
		    </ul>    
	    </header>    
	    <section>    
		    <div id="middle">    
			    <p><u><i>This is middle section</i></u></p>    
			    <p>I am description</p>    
		    </div>    
	    </section>    
	    <footer>    
		    <p>This is footer</p>    
	    </footer>    
    </div>           


<br>

Answer::  ***Don't look first***
	
	
    div>(header>h2{Header $$}*3+p{This is a paragraph.}+ul.nav>li#list${List $$$}*4)+(section>div#middle>p>u>i{This is middle section}^^p{I am description})+footer>p{This is footer}
