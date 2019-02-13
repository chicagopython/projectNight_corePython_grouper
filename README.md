# Core Python Grouping Exercise

## How you should think about this exercise
- core python data structures are invaluable
- object-oriented programming is encouraged for this problem
- built-in and 3rd party libraries are useful if you understand them
- building small components is a great way to understand high level
  abstractions

## Problem:
grouping people for an exercise like this is challening. For our purposes, the most
important problems are:
- group size
- skill levels of people in the group

**the goal** is to achieve an even distribution of skill level for each group

## Assumptions:
- people may be referenced by any string identifier, e.g., ``"AA"`` or ``"B789ghk"`` or ``"Dana"``
- people provide their own score for their comfort with core python, an integer
  from ``0`` to ``100``
- each person has one score
- people **can** have the same identifier
- the `random` module is the only recommended module to import.

## Objectives:
### 1a) generate an integer determining the number of attendees, typically
turnout is between 35 and 50
### 1b) build a method which generates an identifier for each person in
attendance, e.g., ``"AA"`` or ``"B789ghk"`` 
### 1c) build a method which generates a score for each person in attendance
### 2) create a data structure which associates a person with a score. Hint: after this step you may elect to store this association locally to confirm consistent results later on. 
### 3) create groups of almost all equal sizes (up to 2 groups of 5 or one
group of 3 is okay). The goal is to maximize the distribution of python skill
level across all groups, i.e., beginners might be paired with advanced people.
### 4) Extra challenges:
- build a method to ``add`` a single participant at once
- build a method to ``add_many`` participants at once
- build a method to ``remove`` a participant
- build a method to ``list`` all participants
