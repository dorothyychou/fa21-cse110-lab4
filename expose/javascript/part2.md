# Intro to Javascript - Part 2
<ol>
    <li>At line 12, the length of the array prices, which is 3, is printed to the console. Since variable i is declared with the var keyword, it has no block scope so it can be accessed outside the for loop and so i is the value that it was at the end of the for loop (which is 3, the length of array prices).</li>
    <li>At line 13, the value of discountedPrice, which is 150, is printed to the console. Like for #1, the variable discountedPrice is declared with the var keyword so it can be accessed outside the for loop. Thus, the last value discountedPrice is set to is what is printed at line 13. The last value would be the discounted price for the last price in the prices array, which is 300, so with the discount it is 150.</li>
    <li>At line 14, the value of finalPrice, which is 150, is printed to the console. Similar to #1 and #2, finalPrice is declared with the var keyword so it can be accessed outside the for loop. At line 14, finalPrice holds last value that was pushed to the discounted array which is also the discounted price of the last price in the prices array, so 150.</li>
    <li>This function returns an array of the discounted versions of the prices in the prices array using the discount determined by the variable discount. So for prices array = [100,200,300], this function would return [50,100,150].</li>
    <li>At line 12, there would be a reference error because i is declared with the let keyword and not defined outside its block scope, which would be the for loop at lines 6-10.</li>
    <li>At line 13, there would be a reference error because discountedPrice is declared with the let keyword inside the for loop at lines 6-10, so line 13 is outside the variable discountedPrice's block scope so it cannot be accessed there.</li>
    <li>At line 14, the value of finalPrice, which is 150, is printed to the console. Although finalPrice is declared with the let keyword, similar to in #5 and #6, it is declared outside the for loop so its block scope is the entire function discountPrices and it can be accessed anywhere within the function. Thus, at line 14, the last value it is set to inside the for loop, 150, is printed.</li>
    <li>This function returns an array of the discounted versions of the prices in the prices array using the discount determined by the variable discount just like in #4. For prices array = [100,200,300], this function would return [50,100,150]. Changing all the variable declarations from using var to using let did not make a difference in what this function returned since each variable can still be accessed where they are each needed.</li>
    <li>At line 11, there is a reference error since i was declared with the let keyword in the for loop at lines 6-9. So line 11 is outside its block scope and it cannot be accessed there.</li>
    <li>At line 12, the value of length, which is 3, is printed to the console. The variable length is declared as a constant variable and set to the length of the prices array on line 4 and is not changed throughout the function, so printing length would just print the length of the prices array, which is 3 for this example.</li>
    <li>This function returns an array of the discounted versions of the prices in the prices array using the discount determined by the variable discount just like in #4 and #8. For prices array = [100,200,300], this function would return [50,100,150]. Using the const keyword when declaring some variables did not make a difference in what the function returned because all the variables could still be changed or accessed where they needed to be.</li>
    <li>
        <ol type="A">
            <li>student.name</li>
            <li>student["Grad Year"]</li>
            <li>student.greeting</li>
            <li>student["Favorite Teacher"].name</li>
            <li>student.courseLoad[0]</li>
        </ol>
    </li>
    <li>
        <ol type="A">
            <li>'32'. '3' is a character so adding an integer 2 means 2 will be mapped to its string representation and concatenated with '3'.</li>
            <li>1. The string '3' is converted to an integer because subtraction - is being applied to it so 3-2=1.</li>
            <li>3. The null maps to integer 0 so 3+null=3+0=3.</li>
            <li>'3null'. The null maps to the string 'null' and then is concatenated with the string '3' so it becomes '3null'.</li>
            <li>4. true maps to integer 1 so 1+3=4.</li>
            <li>0. false maps to integer 0 and null also maps to integer 0 so 0+0=0.</li>
            <li>'3undefined'. undefined maps to the string 'undefined' and then it is concatenated with string '3' so '3undefined'.</li>
            <li>NaN. '3' maps to the integer 3 and then subtracting an undefined value results in NaN which is not-a-number.</li>
        </ol>
    </li>
    <li>
        <ol type="A">
            <li>true. '2' maps to the integer 2 and 2>1 is true.</li>
            <li>false. The string '2' is larger compared to the string '12' because they are compared character by character and '2'<'1' is false.</li>
            <li>true. The == operator converts the values to the same type before comparing so '2' could map to the integer 2 and 2 is equal to 2 so 2=='2' is true.</li>
            <li>false. The === operator does not convert the values to the same type before comparing, so 2==='2' is false.</li>
            <li>false. == converts the values to the same type, so true could map to integer 1, but 1 does not equal 2 so this is false.</li>
            <li>true. Boolean(x) where x is a nonzero value is true so true===true is true.</li>
        </ol>
    </li>
    <li>The == operator converts the values to the same type before comparing so as long as the values are equal after being converted to the same type it would return true. Whereas the === operator does not convert the values to the same type before comparing so it only returns true if the two sides are the same type and the same value.</li>
    <li>In file part2-question16.js.</li>
    <li>The result would be [2,4,6]. This is because when we call modifyArray with array [1,2,3] and callback doSomething, we push each element of array onto the new array (newArr) after sending them through the callback function. So we would push doSomething for each element of array. Thus, [1,2,3] becomes [2,4,6] because in doSomething each element is doubled.</li>
    <li>In file part2-question18.js.</li>
    <li>
    1 <br>
    4 <br>
    3 <br>
    2
    </li>
</ol>