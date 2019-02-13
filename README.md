# Core Python Grouping Exercise

## How you should think about this exercise
- core Python data structures are invaluable
- object-oriented programming is encouraged for this problem
- built-in and 3rd party libraries are useful if you understand them
- building small components is a great way to understand high level
  abstractions
- instructions are often open-ended

## Problem:
This is a meta-exercise: the project is to optimally group
people of different skils together for an event such as project night.
Further, to make it challenging, the goal is to use Core Python and no
imported libraries (except for [`random`][random]).

Grouping people for an exercise like this is challening. For our purposes, the most
important constraints are:
- group size
- skill levels of people in the group

**the goal** is to achieve an even distribution of skill level for each group.

## Assumptions:
- people may be referenced by any string identifier, e.g., ``"AA"`` or ``"B789ghk"`` or ``"Dana"``
- people provide their own score for their comfort with core python, an integer
  from ``0`` to ``100``, including both end points
- each person has one score
- people **can** have the same identifier
- the [`random`][random] module is the only recommended module to import (and maybe [`string`][string] depending on how you generate identifiers)
- group size is 4

## Objectives:

1) Setup
    1) Generate an integer determining the number of attendees, typically turnout is between 35 and 50
    2) Build a method which generates an identifier for each person in attendance, e.g., "AA" or "B789ghk"
    3) Build a method which generates a score for each person in attendance
2) Create a data structure that associates a person with a score.
    - Hint: because we are using random numbers, you may elect to write the generated data to a file to make it possible to re-run and confirm consistent results during the later steps.
    - Hint: it may be useful to define a [``__repr__``][repr] method so you can see what is happening when you print the data structure.
3) Create groups of almost all equal sizes (up to 2 groups of 5 or one group of 3 is okay). The goal is to have an even distribution of Python skill level across all groups, i.e., beginners could be paired with advanced people so the average group score is nearly constant.
    - Hint: `help(sorted)` may be useful when making sorted lists of data structures
4) Extra challenges:
    1) build a method to ``add`` a single participant at once
    2) build a method to ``add_many`` participants at once
    3) build a method to ``remove`` a participant
    4) build a method to ``list`` all participants
    5) build a method to evaluate the distribution of skill levels across all groups


[data structures]: https://docs.python.org/3/tutorial/datastructures.html
[random]: https://docs.python.org/3.7/library/random.html
[repr]: https://docs.python.org/3/reference/datamodel.html#object.__repr__
[string]: https://docs.python.org/3.7/library/string.html#string.ascii_letters
