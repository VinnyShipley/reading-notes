# Ten Thousand Game 1

## Random Module

### The random module allows you to generate random numbers

### Random functions

* Randint

  * The randint function takes in two parameters, a low and a high bound. The function then picks a random number between the two parameters. The lower bound should always go on the left of the right one.

* Choice

      random.choice([red, black, green, purple])
  
  The code above will choice a random color from the given list.

* Shuffle

  * Using the shuffle method, a presorted list can be shuffled into a random order

        shuffle(list_variable_name_here)

* Randrange

  * Given a start, a stop and a step value, find a randomly selected value using those parameters. The code below will choose a random integer between 0 and 101, using a step of 5

        random.randrange(0, 101, 5)

## Risk Analysis

### Definition: In software testing, risk analysis is the process of identifying the risks in applications or software that you built and prioritizing them to test

### Why Use Risk Analysis

Using risk analysis at the beginning of the process highlights potential problem areas. With that in mind, more thoughtful and efficient testing can happen during the coding process

Certain risks are unavoidable:

* Time allocated for testing

* A defect in the product due to the size or complexity of the app

* Urgency from the client

* Incomplete requirements

### Risk Magnitude

* High: The effect of the risk would be very high an non-tolerable. Company has a chance to face loss

* Medium: Tolerable, but not desireable. Company could lose money, but that risk is limited

* Low: Tolerable risk. little to no external exposure or financial loss

### Risk Identification

* Business risk: This risk is the kind that comes from the company or customer, ot the project

* Testing risk: Risks that will arise during the testing process

* Premature release risk: The risk associated with releasing an unfinished project, or one that is untested

* Software risk: Risks associated with the development of the software construction

### Risk Assessment

There are three perspectives in risk assessment

* Effect: To assess the risk by what the impact of the potential problem will be

* Cause: To assess the risk by what the potential cause of the risk could be

* Likelihood: To assess the risk that the problem will occur

## Test Coverage

### Test coverage is a tool to help you find untested code within your codebase

Good test coverage isn't necessarily a static number, it moves with each project and depends on the quality of the tests being done that contribute to the test coverage quotient.

Good test coverage means that bugs will rarely escape into production, as well as facilitates more dynamic code production, as devs aren't worried about changing the code base for fear of production bugs.

You can test too much if you have the ability to remove tests and still have enough, or if writing tests is slowing you down too much.

## Big O Notation

There are multiple ways to describe O(N), as long as you describe what the variable is representing. S could represent the same thing as 5N, what matters is describing the value of the variable in relation to the algorithm.
c