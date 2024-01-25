[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/GDPVb20V)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```

# Answer
In the big picture this code just finds the maximum value in the array. In more detail this code recursivly slices the array into pieces and then compares each piece and then returns the larger one. It then checks the next slice "up" the recursive chain and returns the largest and then keeps repeating this until it returns the largest value in the array.