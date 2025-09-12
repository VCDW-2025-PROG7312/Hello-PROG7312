## Simple Tree Data Structure - Organizational Tree
To learn about the tree data structure, build an app that allows storing and displaying of represents an organizational hierarchy using a generic tree data structure. The hierarchy will consist of a CEO and C-suite executives (CIO, CFO, COO, CTO), each with their own direct reports. Implement this system in C#.
 
You are welcome to use any resources of your choice including the guru playlist and PROG7312 bot.
 
Here is a sample hierarchy:
* CEO: Zanele
    * CIO: Thabo
        * Software Development Manager: Linda
        * Developer: Lindiwe
    * CFO: Pieter
        * Accountant: Muhammad
    * COO: Lerato 
        * Operations Manager: Nomsa
    * CTO: Sifiso
        * Tech Lead: Megan

## Tree Traversal
There are multiple ways to traverse a tree and search a tree - read up on them.

Then,
* Add in the ability to search the tree for an employee.
* Add in the ability to traverse the tree in the following ways:
 
### Pre-order Traversal (top to bottom)
So I can view each person and their direct reports all the way down
* CEO: Zanele
    * CIO: Thabo
        * Software Development Manager: Sipho
        * Developer: Lindiwe
    * CFO: Pieter
        * Accountant: Muhammad
    * COO: Lerato
        * Operations Manager: Nomsa
    * CTO: Sibusiso
        * Tech Lead: Megan
 
### Post-order traversal (bottom to top)
So I can view each person and their managers all the way up
* Developer: Lindiwe
    * Software Development Manager: Sipho
        * CIO: Thabo
* Accountant: Muhammad
    * CFO: Pieter
* Operations Manager: Nomsa
    * COO: Lerato
* Tech Lead: Megan
    * CTO: Sibusiso 
* CEO: Zanele 
 
### Level-order Traversal (Breadth-First to achieve level by level)
So I can view level by level which is useful to view all executives, all managers, etc.
* CEO: Zanele
    * CIO: Thabo
    * CFO: Pieter
    * COO: Lerato
    * CTO: Sibusiso 
        * Software Development Manager: Sipho
        * Accountant: Muhammad
        * Operations Manager: Nomsa Gcaba
        * Tech Lead: Megan Botha
            * Developer: Lindiwe Ndlovu

## Tree searching

Implement a searching algorithm for your tree.