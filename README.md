# Ruby Instance Variable Modification Bug

This repository demonstrates a subtle bug in Ruby related to how instance variables are modified through getter methods.

The `bug.rb` file contains code that showcases the unexpected behavior.  The `bugSolution.rb` file provides a solution.

## Bug Description

In Ruby, it's common to create getter methods to access instance variables. However, directly assigning a value to a getter method will not modify the instance variable unless it's specifically designed to allow such behavior.  This can lead to confusion and unexpected results.

## Solution

The solution involves creating a `setter` method to explicitly modify the instance variable.