---
theme: test_design
title: Three parts of a test
kata: calc_stats
difficulty: 1
author: emilybache
affiliation: ProAgile
---

# Three parts of a test

This learning hour is about Arrange - Act - Assert and uses a simpler exercise than [AAA](arrange_act_assert.html).

### Learning Goals

- recognize a well-structured test case.
- use the three parts when designing a test case.

## Session Outline

* 5 min connect: What is an automated unit test  
* 10 min concept: Three parts of a test  
* 35 min concrete: Write some tests 
* 5 min conclusions: When to do this


### Connect: Three facts
What is an automated unit test? Give me [three facts](/activities/connect/three_facts.html) about it.

### Concept: Three parts of a test
An automated test usually has three kinds of code.

* _Arrange_ - set up the test data and environment your function will need
* _Act_ - exercise the function you want to test
* _Assert_ - verify it did the right thing by checking what happened

Normally in a unit test you only have one of each section, and they come in that order. If you want to check another thing, add a new test case. Don’t just build more act-assert steps onto the same test case.

### Concrete
Write some test cases for some existing code that already basically works. For example [CalcStats](/kata_descriptions/calc_stats.html). Be sure to structure your test cases using Arrange - Act - Assert. If you find any bugs in the code, please fix them.

### Conclusions
Can you think of any advantages of structuring your tests this way, with Arrange - Act - Assert? Are there any situations where it wouldn’t be a good idea? [When should you use this?](/activities/conclusions/when_to_use_this.html)
