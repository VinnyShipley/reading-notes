# Functional Programming

## Functional Programming Concepts

1. **What is functional programming?** Functional programming is the idea that computation is the evaluation of mathematical functions and avoids the mutation of data. I think this essentially means focusing on the processes and how they affect the objects within computing within the computation rather than strictly the objects themselves.

2. **What is a pure function and how do we know if something is a pure function?** A pure function is a function that returns the same result if given the same arguments, as well as not having any observable side efects.

3. **What are the benefits of a pure function?** One benefit is that the result will always be static, and not change based on external factors.

4. **What is immutability?** Immutability is a property that, if possessed by a variable, means that it's state cannot be changed after it's been created.

5. **What is referential transparency?** referential transparency is a property that, if possessed by a function, means that it will consistently yieald the same result for the same input.

## Video

1. **What is a module?** A way of separating up functionality within an app so that it is easier to organize and hand off to another developer in the future. It is essentially another javascript file that functionality lives in and is referenced.

2. **What does the word ‘require’ do?** It creates a path to a different module for an application to use.

3. **How do we bring another module into the file the we are working in?** You bring in the file by passing it's path in as a string to the argument of the require function.

4. **What do we have to do to make a module available?** You have to require the module, and then specify what part of the module you want to reference in the javascript file it's going to, as well as declaring it as an export with module.exports being set to whatever function you want exported within the exporting file.
