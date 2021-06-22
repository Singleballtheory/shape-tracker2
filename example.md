return an array from 0 to inputed number
If number in array includes 1, replace with Beep
If number in array includes 2, repalce with Boop, even if it also has 1
If number in array includes 3, replace with Won't you be my neighbor, even if it has a 1 and/or 2



Describe: function beepBoop()
Test: It should return an array from 0 to the inputed number
Code: beepBoop(6)
Expected: [0,1,2,3,4,5,6]

function beepBoop(input) {
  let array = []
  for (i = 0; i <= input; i++){
    array.push(i)
  }
  return array
}

```
Test: If any number in array includes 1, it should replace with "Beep"
Code: beepBoop(11)
Expected: [0,"Beep",2,3,4,5,6,7,8,9,"Beep","Beep"]

function beepBoop(input) {
  let array = [];
  for (i = 0; i <= input; i++) {
    if (i.toString().includes("1")) {
      array.push("Beep");
    } else {
    array.push(i);
    }
  };
  return array;
};

