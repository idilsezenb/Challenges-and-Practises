#HackerRank 10 Days Javascript Challenge

##Day 3:Intro to Conditional Statements
You can find the code in the challenge with its explanations.

//**************Code start*************
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
    //***************This is where you need to write the code***********************
    
    if (N%2 == 1) { console.log("Weird");} //Here we use the "% (mode)" operator to indicate whether "N" is odd or even.
  
    else if ( (N%2 == 0) && (2 <= N <= 5) ) {console.log("Not Weird");} //Here we look at whether "N" is even and between 2 and 5.
    
    else if ( (N%2 == 0) && (6 <= N <= 20) ) {console.log("Weird");} //Here we look at whether N is even and between 6 and 20.
    
    else if ( (N%2 == 0) && (N > 20) ) {console.log("Not Weird");}//Here we look at whether N is greater than 20.
    
    }
