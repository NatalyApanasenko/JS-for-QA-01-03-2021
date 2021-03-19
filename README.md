2.1 

let schedule = {};

const isEmpty = (obj) => {
    for (let key in obj) {
      return false;
    }
    return true;
  }

  console.log( isEmpty(schedule) ); 
  schedule["8:30"] = "get up";
  console.log( isEmpty(schedule) );

2.2. 

function maxNumber (a, b) {
return Math.max(a,b)
}
  console.log(maxNumber (1, 2))

3.

let salaries = { 
    workers: {
    Mykola: 950,
    Pavlo:  700, 
    Petro:  800,
    Helen: null
    },
    culcSumm: () => {
        let result = 0; 
        for (let key in salaries.workers){
    //  if ((this.workers)[key] != null){
            result += (salaries.workers)[key]
    // } 
        }
        return result
    },

    topSalaries: function() {
        let max = 0;
        let name = null;

        for (const [employee, salary] of Object.entries(salaries.workers))  {
            if (max < salary){
                max = salary;
                name = employee;
            }
        }
        // for (let key in this.workers) {
        //     max = Math.max ((this.workers)[key], max);
        
        return `${name} has biggest salary of ${max}`;
        // return max
    }
}
console.log(salaries.culcSumm())
console.log(salaries.topSalaries())


4.

let menu = { 
      width: 200, 
      height: 300, 
      title: "My menu" 
    };
    
    const multiplyNumeric = (obj) => {
        for (let key in obj) {
          if (typeof obj[key] == 'number') {
            obj[key] *= 2;
          }
        }
      }

  multiplyNumeric(menu)

  menu

5. 

function showStars(rows){
    let star ='';
    for (let row = 1; row <= rows; row++ ){
           for(let i = 1; i <= rows - row ; i++) {
            star += "\t";
     } 
     for (let a = 1; a <= row; a++){
         star += '*\t\t';
     }
     console.log(star);
     star = ""; 
    }
}
   showStars(4)
