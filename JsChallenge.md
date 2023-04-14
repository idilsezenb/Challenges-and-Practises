# HackerRank 10 Days Javascript Challenge
You can find the codes in the challenges with its explanations.

## Day 3:Intro to Conditional Statements

<br>
'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', function(inputStdin) {
    inputString += inputStdin;
});

process.stdin.on('end', function() {
    inputString = inputString.split('\n');

main();
});

function readLine() {
    return inputString[currentLine++];
}



function main() {
    const N = parseInt(readLine().trim(), 10);  
    **Down from here is where you need to write the code**
    
    if (N%2 == 1) { console.log("Weird");}  //Here we use the "% (mode)" operator to indicate whether "N" is odd or even.  
  
    else if ( (N%2 == 0) && (2 <= N) && (N <= 5) ) {console.log("Not Weird");} //Here we look at whether "N" is even and between 2 and 5.
    
    else if ( (N%2 == 0) && (6 <= N) && (N <= 20) ) {console.log("Weird");}  //Here we look at whether N is even and between 6 and 20.  
    
    else if ( (N%2 == 0) && (N > 20) ) {console.log("Not Weird");}  //Here we look at whether N is greater than 20.  
    
    }


## Day 2: Conditional Statements: Switch

<br>

'use strict';

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', inputStdin => {
    inputString += inputStdin;
});

process.stdin.on('end', _ => {
    inputString = inputString.trim().split('\n').map(string => {
        return string.trim();
    });
    
    main();    
});

function readLine() {
    return inputString[currentLine++];
}

function getLetter(s) {
 **Down from here is where you need to write the code**
   switch(s.charAt(0)) {   //charAt fetches the property at the specified address.
       case('a' || 'e' || 'i' || 'o' || 'u'):   //Parentheses are used for multiple selections. "||" means 'or'. ":" is put at the end of the case.
       return 'A';
       break; //If we don't write break here, the loop won't stop.
       
       case('b' || 'c' || 'd' || 'f' || 'g'):
       return 'B';
       break;
       
       case('h' || 'j' || 'k' || 'l' || 'm'):
       return 'C';
       break;
       
       case('z' || 'n' || 'p' || 'q' || 'r' || 's' || 't' || 'v' || 'w' || 'x' || 'y'):
       return 'D';
       break;
       
   }
}
