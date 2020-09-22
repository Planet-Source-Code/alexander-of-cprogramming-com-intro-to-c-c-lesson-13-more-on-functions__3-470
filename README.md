<div align="center">

## Intro to C/C\+\+ Lesson 13: More on Functions


</div>

### Description

The reason I have placed this tutorial at the end of the list, rather than as an addition to my other lesson is simple, I don't want people who already read that tutorial to miss this!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Alexander of CProgramming\.com](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/alexander-of-cprogramming-com.md)
**Level**          |Intermediate
**User Rating**    |4.3 (13 globes from 3 users)
**Compatibility**  |C, C\+\+ \(general\)
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__3-1.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/alexander-of-cprogramming-com-intro-to-c-c-lesson-13-more-on-functions__3-470/archive/master.zip)





### Source Code

<p><font face="Verdana">The reason I have placed this tutorial at the end of the
list, rather than as an addition to my other lesson is simple, I don't want
people who already read that tutorial to miss this!</font></p>
<p><font face="Verdana">In lesson 4 you were given the basic information on
tutorials. However, I left out two items of interest. First, when you declare a
function you don't have to prototype it! However, you must give the function
definition physically before you call the function. You simply type in the
entire definition of the function where you would normally put the prototype.</font></p>
<p><font face="Verdana">For example:</font></p>
<p><font face="Verdana">#include &lt;iostream.h&gt;</font></p>
<p><font face="Verdana">void function(void) //Normally this would be the
prototype. Don't forget to exclude the semicolon</font></p>
<p><font face="Verdana">//Only prototypes have semicolons</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">cout&lt;&lt;&quot;HA! NO PROTOTYPE!&quot;;</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">void main()</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">function(); //It works like a normal function now.</font></p>
<p><font face="Verdana">}</font></p>
<p>&nbsp;</p>
<p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; The other programming concept
is the inline function. Inline functions are not very important, but it is good
to understand them. The basic idea is to save time at a cost in space.</font></p>
<p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; How does an inline function
make the program go faster? How does it make the program larger? Does this
remind you of relativity? Inline functions are really a lot like a placeholder.
Once you define an inline function,using the 'inline' keyword, whenever you call
that function the compiler will replace the function call with the actual code
from the function. How does this&nbsp;make the program go faster? Simple,
function calls are simply more time consuming than writing all of the code
without functions. However, to go through your program and replace a function
you have used 100 times with the code from the function would be time consuming.
Of course, by using the inline function to replace the function calls with code
you will also greatly increase the size of your program.</font></p>
<p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; Using the inline keyword is
simple, just put it before the name of a function. Then, when you use that
function, just pretend it is a non-inline function. For example:</font></p>
<p><font face="Verdana">#include &lt;iostream.h&gt;</font></p>
<p><font face="Verdana">inline void hello(void) //Just use the inline keyword
before the function</font></p>
<p><font face="Verdana">{ //Note that this is a non-prototyed function</font></p>
<p><font face="Verdana">cout&lt;&lt;&quot;hello&quot;;</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">void main()</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">hello(); //Call it like a normal function...</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; However, once the program is
compiled, the call to hello(); will be replaced by the code making up the
function.&nbsp;A WORD OF WARNING: Inline functions are very good for saving
time, but if you use them too often or with large functions you will have a
tremendously large program. Sometimes large programs are actually less
efficient, and therefore they will run slower than before. Inline functions are
best for small functions that are called often.</font></p>
<p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; In the future we will discuss
inline functions in terms of C++ classes. However, now that&nbsp; you understand
the concept I will feel comfortable using inline functions in later tutorials.&nbsp;</font></p>
<p><font face="Verdana">&nbsp;&nbsp;&nbsp;&nbsp; At this point I do not wish to
add something about classes that individuals could easily miss if they did not
realize that the information was in the tutorial.</font></p>

