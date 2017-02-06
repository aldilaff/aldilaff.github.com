---
layout: post
title: Week Three!
---

### What did you do this past week?

This past week I finally finished Collatz getting it to pass Sphere. I then completed the rest of the steps to finish and submit the assignment. One thing I noticed was that running `make Collatz.log` does not update the log file that was created as part of running `make test`. Sadly, I didn’t notice this until I had submitted my JSON file. To fix this isssue, I had to run `git log > Collatz.log` manually and then resubmit my JSON file with the correct new SHA.

### What’s in your way?

Right now, I have to catch up with some readings that I did not get the chance to finish earlier.

### What will you do next week?

I am currently waiting for the new project to be announced. Until then, I will try to catch up with some readings that I missed and hopefully do some of the readings that are assigned for this week. I am hoping to start the new project early just in case I get stuck on any unexpected bugs.

### Class Experience 

On Tuesday, we talked in class about Python’s operations, variables, and copy methods. Some things were very confusing and not intuitive. One example is this part from the [Variables](https://github.com/fareszf/cs373/blob/master/examples/Variables.py) file:
```a = [2, 3, 4]
b = a
assert a is b
b += (5,)
assert a == [2, 3, 4, 5]
assert a is b

a = [2, 3, 4]
b = a
assert a is b
#b = b + (5,) # TypeError: can only concatenate list (not “tuple”) to list```

Somehow, using += to add a tuple to a list works fine. However, adding a tuple to a list using b = b + tuple does not work and raises an error. I asked about this on Piazza and the Professor replied with the explanation: += only requires the right hand side to be an iterable while using + with a list requires the right hand side to be also a list.



### Tip-Of-The-Week

If you are working on more than one python project at the same time and they all have different dependencies, I would recommend looking at [virtualenv](https://virtualenv.pypa.io/en/stable/) which “is a tool to create isolated Python environments.”

