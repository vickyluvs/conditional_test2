# Exercise Link: <br>
https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Test_your_skills:_Conditionals<br>

# Instructions:<br>
For this task you are given three variables:<br>

* `machineActive` - contains an indicator of whether the answer machine is switched on or not <br>
 `(true/false)`<br>
* `score` — Contains your score in an imaginary game. This score is fed into the answer machine, which provides a response to indicate how well you did.<br>
* `response` — begins uninitialized, but is later used to store a response that will be printed to the output panel.<br>

You need to create an `if...else` structure that checks whether the machine is switched on and puts a message into the `response` variable if it isn't, telling the user to switch the machine on.<br>

Inside the first `if...else`, you need to nest another `if...else` that puts appropriate messages into the response variable depending on what the value of score is — if the machine is turned on. The different conditional tests (and resulting responses) are as follows:<br>

* Score of less than 0 or more than 100 — "This is not possible, an error has occurred."<br>
* Score of 0 to 19 — "That was a terrible score — total fail!"<br>
* Score of 20 to 39 — "You know some things, but it\'s a pretty bad score. Needs improvement."<br>
* Score of 40 to 69 — "You did a passable job, not bad!"<br>
* Score of 70 to 89 — "That\'s a great score, you really know your stuff."<r>
* Score of 90 to 100 — "What an amazing score! Did you cheat? Are you for real?"<br>

# My Solution:<br>
```
let response;
    let score = 90;
    let machineActive = false;

    // Add your code here
    if (machineActive) {
      if (score < 0 || score > 100) {
        response = "This is not possible, an error has occurred.";
      } else if (score >= 0 && score <= 19) {
        response = "That was a terrible score — total fail!";
      } else if (score >= 20 && score <= 39) {
        response =
          "You know some things, but it's a pretty bad score. Needs improvement.";
      } else if (score >= 40 && score <= 69) {
        response = "You did a passable job, not bad!";
      } else if (score >= 70 && score <= 89) {
        response = "That's a great score, you really know your stuff.";
      } else if (score >= 90 && score <= 100) {
        response = "What an amazing score! Did you cheat? Are you for real?";
      }
    } else {
      response = "Please turn on the machine to see score";
      score = "loading...";
    }
```
