Download Link: https://assignmentchef.com/product/solved-csc3320-lab-9
<br>
<span class="kksr-muted">Rate this product</span>

<table>

 <tbody>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>

Purpose: Learn how to use array in C. Understand the basic memory address in C.

Part 1:

Write a C program named as getMostFreqChar.c that finds the most frequent letter from the input via ignoring the case sensitive and prints out its frequency. For example, sample outputs could be like below

<pre>$cat test.txt</pre>

This is a list of courses.CSC 1010 – COMPUTERS &amp; APPLICATIONS

$./getMostFreqChar test.txtThe most frequent letter is ‘s’. It appeared 8 times.

Run the C program, attach a screenshot of the output in the answer sheet.

Part 2:

When a variable is stored in memory, it is associated with an address. To obtain the address of a variable, the &amp; operator can be used. For example, &amp;a gets the memory address of variable a. Let’s try some examples.Write a C program addressOfScalar.c by inserting the code below in the main function.

Questions:

1) Run the C program, attach a screenshot of the output in the answer sheet.2) Attach the source code in the answer sheet2) Then explain why the address after intvar is incremented by 4 bytes instead of 1 byte.

<pre>1234567891011</pre>

12

<pre>// intialize a char variable, print its address and the next addresschar charvar = ' ';printf("address of charvar = %p
", (void *)(&amp;charvar));printf("address of charvar - 1 = %p
", (void *)(&amp;charvar - 1));printf("address of charvar + 1 = %p
", (void *)(&amp;charvar + 1));</pre>

<pre>// intialize an int variable, print its address and the next addressint intvar = 1;printf("address of intvar = %p
", (void *)(&amp;intvar));printf("address of intvar - 1 = %p
", (void *)(&amp;intvar - 1));printf("address of intvar + 1 = %p
", (void *)(&amp;intvar + 1));</pre>

<table>

 <tbody>

  <tr>

   <td></td>

   <td></td>

  </tr>

 </tbody>

</table>

Part 3:Write a C program addressOfArray.c by inserting the code below in the main function.

<pre>1234567891011</pre>

12

<pre>// initialize an array of intsint numbers[5] = {1,2,3,4,5};int i = 0;</pre>

<pre>// print the address of the array variableprintf("numbers = %p
", numbers);</pre>

<pre>// print addresses of each array index</pre>

<pre>do {    printf("numbers[%u] = %p
", i, (void *)(&amp;numbers[i]));    i++;</pre>

<pre>} while(i &lt; 5);</pre>

<pre>// print the size of the arrayprintf("sizeof(numbers) = %lu
", sizeof(numbers));</pre>

Questions:

1) Run the C program, attach a screenshot of the output in the answer sheet.

2) Check the address of the array and the address of the first element in the array. Are they the same?