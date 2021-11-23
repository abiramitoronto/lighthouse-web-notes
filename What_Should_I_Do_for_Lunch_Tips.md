### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.


``` javascript
const whatToDoForLunch = function(hungry,availableTime) {
  console.log("hungry is", hungry);
  console.log("availableTime is", availableTime);
  if (hungry) {
    if (availableTime < 20) {
      return "pick something up and eat in back in the Lab or in the kitchen.";
    }
    if (availableTime >= 20 && availableTime < 30) {
      return "you deserve a break and could try a place in Gastown.";
    }
    if (availableTime > 30) {
      return "this is a bootcamp after all and you should probably reconsider.";
    }
  } else {
    return "wait until you're hungry.";
  }
};
console.log(whatToDoForLunch(true,20));
console.log(whatToDoForLunch(true,25));
console.log(whatToDoForLunch(false,25));
console.log(whatToDoForLunch(true,40));
console.log(whatToDoForLunch(true,15));
```
