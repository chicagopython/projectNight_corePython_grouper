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
- people **can** have the same name
- the `random` module is the only recommended module to import.

## Objectives:
### 1a) build a component which generates person identifiers (see Assumptions) 
### 1b) build a component which generates scores 
### 2) associate people with scores. Hint: after this step you may elect to
log the output of people and their scores, then store this object locally to confirm consistent results
### 3) 
