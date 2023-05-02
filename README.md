Download Link: https://assignmentchef.com/product/solved-comp1410-lab-4-pointers
<br>
Learn to use pointers.

<ol>

 <li>Consider the following C program. Assume that memory addresses are expressed in decimal numbers and an integer takes 4 bytes. Also, assume <strong>ids = &amp;ids[0] = 2000</strong>. What would be printed by the following program? Do NOT compile and execute this program as it will not provide the correct results – do the tracing of the program <u>by hand</u> and using only the assumptions stated.</li>

</ol>

<strong>#include &lt;stdio.h&gt; int main(){ int ids[3] = {100,200,300}; int *salary, salary1, salary2, *salary3; salary1 = ids[0] * ids[1]; salary = &amp;ids[1] ;       salary2 = *(ids+1)* *(ids+2); salary3 = ids+2; printf(“*salary = %d
salary1 = %d
”, *salary, salary1); printf(“salary2 = %d
salary3 = %p
”, salary2, salary3); </strong>

<strong>} </strong>

<ol start="2">

 <li>Write a documented function called <strong>Largest </strong>that finds and returns the <strong>address of the largest element </strong>in the array passed to it. (Assume an integer array of size 10). You must use <strong>pointer arithmetic on the array name </strong>instead of the array subscript notation to implement the function. (NOTE: This function will be included as part of step 4 below.)</li>

</ol>

int *Largest( int *array, int size );

<ol start="3">

 <li>Write a documented function called <strong>Swap </strong>that takes two integer <strong>pointers </strong>and exchanges the values of each. It returns void. Example: given two integers ‘a = 2’ and ‘b = 4’, after <strong>Swap (&amp;a, &amp;b) </strong>is called, ‘a’ will be 4 and ‘b’ will be 2. (NOTE: This function will be included as part of step 4 below.)</li>

</ol>

void Swap( int *x, int *y );

<ol start="4">

 <li>Write a complete, well documented C language program (called <strong>c</strong>) to test both the functions <strong>Largest </strong>and <strong>Swap</strong>. In order to test your functions you will need to define and populate an array, within main, that you can pass to <strong>Largest,</strong> and also</li>

</ol>

two initialized int variables to pass into  <strong>Swap</strong>; do not forget to write printf() statements to show Before/After views of any data that will undergo changes.  Ensure that your testing clearly demonstrate each function and its required result.  There is no need for a menu, nor for the program logic to repeat itself (unless you choose to implement such logic).