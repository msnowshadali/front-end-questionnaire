# interview
Front End Interview Questionnaire 

Currying
Example 1
```
function sum(num) {

    if (num === undefined) {
        return 0;
    }

    return (nextNum) => {
        if (nextNum === undefined) {
            return num;
        }
        return sum(num + nextNum);
    }
}

console.log(sum(1)(2)(3)(3)());
```


Example 2
```
function sum(a, b){

    if(b===undefined){
        return (b)=>{
            return a+b;
        }
    }

    return a + b;
}

sum(1,2);
sum(1)(2);
```
