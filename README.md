# Friend-or-Foe

## Problem 

Make a program that filters a list of strings and returns a list with only your friends name in it.

If a name has exactly 4 letters in it, you can be sure that it has to be a friend of yours! Otherwise, you can be sure he's not...

Ex: Input = ["Ryan", "Kieran", "Jason", "Yous"], Output = ["Ryan", "Yous"]

i.e.

friend ["Ryan", "Kieran", "Mark"] `shouldBe` ["Ryan", "Mark"]
Note: keep the original order of the names in the output.

## Solution 1
```javascript
const friend = (friends) => {
   /*
  I want go through array look to see if name equals to 
  three or more words
  
  so I would go through array["jacob", 'tommy', 'john', 'mike']
  if the name in the array has four letters I would then pull it
  out of the array 
  
  to do that I would create an empty variable to push the filtered name
 
  I then would run a for loop over the friends parameter
  or I can use the filter method 
  */
//   create empty array
  store = [];
  
//   run for-loop
  
  for(let i of friends) {
    if(i.length == 4) {
      store.push(i);
    }
  }
  return store;
};
```

## Solution 2
```javascript
const friend = (friends) => {
  const result = friends.filter((word) => word.length == 4);
  return result;
};
```
