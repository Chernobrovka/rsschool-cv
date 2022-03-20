# Dmitry Homan

**Trainee Web Developer**

****

# Contact information:

* Phone: +375444950254
* E-mail: gomhu72@gmail.com
* Telegram: https://web.telegram.org/@Chernobrovka1
* LinkedIn: https://www.linkedin.com/in/dima-goman-9818a7229/

****
# Education:

* Belarusian State Technology University
* 2020-2024
* Automation Engeneer

****

# Languages:

* Russian
* English (A2)

****

# Briefly About Myself:

In 2020, he entered the University of Technology with a degree in automation of technological processes. In 2021, I studied and did projects in the development of embedded systems and automation. Since 2022, I have been developing in the field of front-end development.

****
# Skills:

* HTML5, CSS3
* JavaScript
* Git, GitHub, Basics of OOP
* C/C++ (for Embedded systems), Electronics

****

# Courses:

* JavaScript Manual on learnjavascript.ru
* JS / Html / CSS on CodeBasics
* RS-School stage 1 (in progress)

****


# Code Example:

**The solution to the task CodeWars:**

**Task( 6 Kui ):** You will be given a list of objects. Each object has type, material, and possibly secondMaterial. The existing materials are: paper, glass, organic, and plastic.

Your job is to sort these objects across the 4 recycling bins according to their material (and secondMaterial if it's present), by listing the type's of objects that should go into those bins.

```
function recycle(array) {
  var arr_materails=['paper','glass','organic','plastic'];  
  var arr_baskets=[];
  for(let j=0;j<4;j++) {
    arr_baskets.push(new Array());
  }
  array.forEach(function callback(elem, i, arr) 
  {
    for(let j=0;j<4;j++) 
    {
      var needAddToBasket = false;
      if (elem.material === arr_materails[j])  {
        needAddToBasket = true;
      }
      if (elem.hasOwnProperty ('secondMaterial')) {
        if (elem.secondMaterial === arr_materails[j]) {
          needAddToBasket = true;
        }
      }
      if(needAddToBasket) {
        arr_baskets[j].push(elem.type);
      }
    }
  });
  return arr_baskets;
}

```