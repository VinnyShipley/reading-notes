# Debugging

**Order of Execution** 

Knowing the order in which functions operate is an important part of debugging. By knowing the order, one can more effectively track down where exactly a bug is occuring within the code

Steps of Operation in a function:

1. The function is declared
2. The initial function fires
3. Any subfunction within that initial function is fired
4. The first function interperets the data given to it by the subfunction or subfunctions and completes itself
5. The output of the entire function is given

**The Stack**

As JavaScript works its way through the order of operations, it stacks what data it needs in terms of what it can and cannot render at any given time. This essentially that the mostly deeply nested function will complete first, giving the parent functions the data they need to fully render.

**Hoisting** 

Hoisting is the process that JavaScript does, where it essentially figures out all the processes on the page that it needs to figure out on it's first pass through, and then executes them on the next pass through.

**Error Types**

[Here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error) is a handy MDN page on all the types of errors.
