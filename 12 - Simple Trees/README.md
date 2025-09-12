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

Then, add in the ability to traverse the tree in at least the following ways

### In-order traversal - read up on DFS
So I can view each organisational unit all the way to the highest person not already visited:
Developer: Lindiwe
Software Development Manager: Linda
CIO: Thabo
CEO: Zanele
Accountant: Muhammad
CFO: Pieter
Operations Manager: Nomsa
COO: Lerato
Tech Lead: Megan
CTO: Sifiso

Visually:
```
                                        CEO: Zanele (4)
              /                        /                \                       \
   CIO: Thabo (3)           CFO: Pieter (6)         COO: Lerato (8)          CTO: Sifiso (10)
        |                          |                        |                       |
Software Dev: Linda (2) Accountant: Muhammad (5) Ops Manager: Nomsa (7) Tech Lead: Megan (9)
       |
Developer: Lindiwe (1)
```
> Note: Numbers in parentheses show the order each node is visited.

### Pre-order Traversal (top to bottom) - read up on DFS
So I can view each person and their direct reports all the way down:
CEO: Zanele
CIO: Thabo
Software Development Manager: Linda
Developer: Lindiwe
CFO: Pieter
Accountant: Muhammad
COO: Lerato
Operations Manager: Nomsa
CTO: Sifiso
Tech Lead: Megan

Visually:
```
                                        CEO: Zanele (1)
              /                        /                \                       \
   CIO: Thabo (2)           CFO: Pieter (5)         COO: Lerato (7)          CTO: Sifiso (9)
        |                          |                        |                       |
Software Dev: Linda (3) Accountant: Muhammad (6) Ops Manager: Nomsa (8) Tech Lead: Megan (10)
       |
Developer: Lindiwe (4)
```
> Note: Numbers in parentheses show the order each node is visited.

### Post-order traversal (bottom to top) - read up on DFS
So I can view each person and their managers all the way up:
Developer: Lindiwe
Software Development Manager: Linda
CIO: Thabo
Accountant: Muhammad
CFO: Pieter
Operations Manager: Nomsa
COO: Lerato
Tech Lead: Megan
CTO: Sifiso
CEO: Zanele

```
                                        CEO: Zanele (10)
              /                        /                \                       \
   CIO: Thabo (3)           CFO: Pieter (5)           COO: Lerato (7)          CTO: Sifiso (9)
        |                          |                        |                       |
 Software Dev: Linda (2) Accountant: Muhammad (4) Ops Manager: Nomsa (6)    Tech Lead: Megan (8)
        |
 Developer: Lindiwe (1)
```
> Note: Numbers in parentheses show the order each node is visited.

### Level-order Traversal (Breadth-First to achieve level by level)
So I can view level by level which is useful to view all executives, all managers, etc.
CEO: Zanele
CIO: Thabo, CFO: Pieter, COO: Lerato, CTO: Sifiso
Software Development Manager: Linda, Accountant: Muhammad, Operations Manager: Nomsa, Tech Lead: Megan
Developer: Lindiwe

Visually:
```
 Level 1:  CEO: Zanele (1)

 Level 2:  CIO: Thabo (2)   CFO: Pieter (3)   COO: Lerato (4)   CTO: Sifiso (5)

 Level 3:  Software Dev: Linda (6)   Accountant: Muhammad (7) 
           Operations Manager: Nomsa (8)   Tech Lead: Megan (9)

 Level 4:  Developer: Lindiwe (10)
```
> Note: Numbers in parentheses show the order each node is visited.

## Tree searching

Implement a searching algorithm for your tree. Research the various searching algorithms that you might apply to trees.

Then, add in the ability to search the tree for an employee.