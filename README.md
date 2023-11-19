 function calculator(string) {
    let q = string.split(' '); 
    let resultFinal = 0; 
    let Num1 = q[0];  
    let Num2 = q[2]; 
    let operator = q[1]; 

     
    const arrNumRim = { '1':1, '2':2, '3':3, '4':4, '5':5, '6':6, '7':7, '8':8, '9':9, '10':10, '+':'+', '-':'-', '*':'*', '/':'/',} 
    const arrRim = { 'I':1, 'II':2, 'III':3 , 'IV': 4, 'V': 5, 'VI':6, 'VII':7, 'VIII': 8, 'IX': 9,'X':10 ,'+':'+', '-':'-', '*':'*', '/':'/', } 
   
    if(q.length == 3 && Num1 !== ' ' && Num2 !== ' ' && arrNumRim.hasOwnProperty(operator)){ 

   function indeficate (Num1, operator, Num2){ 

    function chooseActive(Num1, operator, Num2) { 

    if(arrNumRim.hasOwnProperty(Num1) && arrNumRim.hasOwnProperty(Num2) && arrNumRim.hasOwnProperty(operator)){ 

    let NumNum1 = Number(Num1); 
    let NumNum2 = Number(Num2); 

    if (operator === '+') { 
    return (result1 = NumNum1 + NumNum2);  
    } else if (operator === '-') { 
    return (result1 = NumNum1 - NumNum2);
    } else if (operator === '*') { 
    return (result1 = NumNum1 * NumNum2);
    } else if (operator === '/') { 
    return (result1 = NumNum1 / NumNum2);
    } else { 
    return console.log('Unknown operator'); 
    } 


  
    } else if (Num1 in arrRim && operator in arrRim && Num2 in arrRim) { 
    let NumNum12 = arrRim[Num1]; 
    let NumNum22 = arrRim[Num2]; 

    if (operator === '+') { 
    return (result1 = NumNum12 + NumNum22);
    } else if (operator === '-') { 
    return (result1 = NumNum12 - NumNum22);
    } else if (operator === '*') { 
    return (result1 = NumNum12 * NumNum22);
    } else if (operator === '/') { 
    return (result1 = NumNum12 / NumNum22);
    } else { 
    return console.error('Unknown operator'); 
    } 

    } else console.error 


    } 
    return result = Math.floor(chooseActive(Num1, operator, Num2)); 
   } 
    let preResult = indeficate(Num1, operator, Num2); 
  
    let prePesultF = preResult.toString();

   function checkStr(Num1, Num2) { 

    const arrNumRimTest = [ '1', '2', '3', '4', '5', '6', '7', '8', '9', '10' ,'+', '-', '*', '/',]; 
    const arrRimTest = [ 'I', 'II', 'III', 'IV', 'V', 'VI', 'VII', 'VIII', 'IX', 'X', '+', '-', '*', '/',]; 
    function NumCheckAndResult(preRes){ 
    if (arrNumRimTest.includes(Num1) && arrNumRimTest.includes(Num2)){ 
    let result2 = preRes.toString(); 
    return result2; 
    } else if (arrRimTest.includes(Num1) && arrRimTest.includes(Num2)){ 
    if(preResult >= 0){ 
    function convertFromRomanNum(prePres){ 
    if(preRes.length == 1){ 
    var numberToRim = { 
    "1": 'I', "2": 'II', "3": 'III', "4": 'IV', "5": 'V', "6": 'VI', "7": 'VII', "8": 'VIII', "9": 'IX' , 
    }, 
    arr = prePres.split(""), 
    numberToRim = arr.map(function (i) { 
    return numberToRim[i] || ''; 
    }); 

    return numberToRim.join(""); 

    }else if(prePres.length == 2 || prePres.length == 3){ 
    var numberToRim = { 
    0 : { "1": 'I', "2": 'II', "3": 'III', "4": 'IV', "5": 'V', "6": 'VI', "7": 'VII', "8": 'VIII', "9": 'IX' ,}, 
    1 : { "1": 'X', "2": 'XX', "3": 'XXX', "4": 'XL', "5": 'L', "6": 'LX', "7": 'LXX', "8": 'LXXX', "9": 'XC' }, 
    2 : { '1':'C',}, 
    }, 
    arr = prePres.toString().split("").reverse(), 
    numberToRim = arr.map(function (a, i) { 
    return numberToRim[i][a] || ''; 
    }); 
    return numberToRim.reverse().join(""); 

    }elseconsole.log("the result is huge") 

       } 
       return convertFromRomanNum(prePesultF); 
       } else console.log(""); 
      }else throw new Error('something went wrong') 

      } 
      return NumCheckAndResult(prePesultF) 
      } 
       resultFinal = checkStr(Num1, Num2); 
       return resultFinal 

    } else console.error(error) 
  }; 

module.exports = calculator; // Не трогайте эту строчку
