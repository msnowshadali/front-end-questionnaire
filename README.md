# interview
Front End Interview Questionnaire 


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

Currying 
