# Intro to Javascript - Part 1
### var declaration
<ol>
<li>Line 9 prints "values added: 20."</li>
<li>Line 13 prints "final result: 20."</li>
</ol>

### let declaration
<ol start="3">
  <li>Line 9 prints "values added: 20."</li>
  <li>The code returns a reference error at line 13 because line 13 is not in the scope of the variable result since the let keyword has block scope and line 13 is not in the same block as where result was declared.</li>
</ol>

### const declaration
<ol start="5">
  <li>Line 9 does not do anything because there is a type error at line 7 that terminates the program. The error is trying to assign a new value to the constant variable result. Result was declared with the const keyword so its value cannot be changed after that. </li>
  <li>Line 13 also does not do anything because the program terminated at the error in line 7. (Same reason as #5).</li>
</ol>