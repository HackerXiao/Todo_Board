# Todo_Board
A board manage multiple todo_lists and iterms.
In phase_1, I created the TodoBoard only manage a single List which contains many Items.
In phase_2, I refactored the code to support the following features:
* marking items as done
* deleting items
* managing multiple lists in a single board

Here is an example of our final product in action:

Enter a command: mklist groceries
Enter a command: mklist tech
Enter a command: ls
 groceries
 tech

Enter a command: mktodo groceries butter 2019-10-24
Enter a command: mktodo groceries milk 2019-10-23
Enter a command: mktodo groceries candy 2019-10-31 sugar-free
Enter a command: mktodo groceries toothpaste 2019-10-29
Enter a command: print groceries
-------------------------------------------------
                GROCERIES
-------------------------------------------------
Index | Item                 | Deadline   | Done
-------------------------------------------------
0     | butter               | 2019-10-24 | [ ]
1     | milk                 | 2019-10-23 | [ ]
2     | candy                | 2019-10-31 | [ ]
3     | toothpaste           | 2019-10-29 | [ ]
-------------------------------------------------

Enter a command: print groceries 2
-------------------------------------------------
candy                           2019-10-31    [ ]
sugar-free
-------------------------------------------------

Enter a command: mktodo tech ruby 2019-10-24
Enter a command: mktodo tech rails 2019-11-02
Enter a command: mktodo tech javascript 2019-11-30
Enter a command: showall
-------------------------------------------------
                GROCERIES
-------------------------------------------------
Index | Item                 | Deadline   | Done
-------------------------------------------------
0     | butter               | 2019-10-24 | [ ]
1     | milk                 | 2019-10-23 | [ ]
2     | candy                | 2019-10-31 | [ ]
3     | toothpaste           | 2019-10-29 | [ ]
-------------------------------------------------
-------------------------------------------------
                TECH
-------------------------------------------------
Index | Item                 | Deadline   | Done
-------------------------------------------------
0     | ruby                 | 2019-10-24 | [ ]
1     | rails                | 2019-11-02 | [ ]
2     | javascript           | 2019-11-30 | [ ]
-------------------------------------------------

Enter a command: toggle groceries 1
Enter a command: toggle groceries 3
Enter a command: toggle tech 2
Enter a command: showall
-------------------------------------------------
                GROCERIES
-------------------------------------------------
Index | Item                 | Deadline   | Done
-------------------------------------------------
0     | butter               | 2019-10-24 | [ ]
1     | milk                 | 2019-10-23 | [✓]
2     | candy                | 2019-10-31 | [ ]
3     | toothpaste           | 2019-10-29 | [✓]
-------------------------------------------------
-------------------------------------------------
                TECH
-------------------------------------------------
Index | Item                 | Deadline   | Done
-------------------------------------------------
0     | ruby                 | 2019-10-24 | [ ]
1     | rails                | 2019-11-02 | [ ]
2     | javascript           | 2019-11-30 | [✓]
-------------------------------------------------