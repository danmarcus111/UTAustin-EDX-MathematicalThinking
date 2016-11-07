# Towers of Hanoi

This puzzle is played with a pyramid of disks (larger at the bottom, smaller at the top) on a 3 column board.  The disks are in a perfect pyramid on one of the side columns and the aim is to move them to the same configuration on the middle column.

The constraints are:

* you can only move one disk at a time;
* you can only take a disk from the top of a column;
* you cannot move a bigger disk on top of a smaller disk;

## Starting point

[]				[]				[5,4,3,2,1]
[1]				[]				[5,4,3,2]
[1]				[2]				[5,4,3]
[]				[2,1]			[5,4,3]
[3]				[2,1]			[5,4]
[3]				[2]				[5,4,1]
[3,2]			[]				[5,4,1]
[3,2,1]			[]				[5,4]
[3,2,1]			[4]				[5]
[3,2]			[4]				[5,1]
[3]				[4,2]			[5,1]
[3]				[4,2,1]			[5]
[]				[4,2,1]			[5,3]
[1]				[4,2]			[5,3]
[1]				[4]				[5,3,2]
[]				[4]				[5,3,2,1]
[4]				[]				[5,3,2,1]
[4,1]			[]				[5,3,2]
[4,1]			[2]				[5,3]
[4]				[2,1]			[5,3]
[4,3]			[2,1]			[5]
[4,3]			[2]				[5,1]
[4,3,2]			[]				[5]
[4,3,2,1]		[]				[5]
[4,3,2,1]		[5]				[]
[4,3,2]			[5]				[1]
[4,3]			[5,2]			[1]
[4,3]			[5,2,1]			[]
[4]				[5,2,1]			[3]
[4,1]			[5,2]			[3]
[4,1]			[5]				[3,2]
[4]				[5]				[3,2,1]
[]				[5,4]			[3,2,1]
[]				[5,4,1]			[3,2]
[2]				[5,4,1]			[3]
[2,1]			[5,4]			[3]
[2,1]			[5,4,3]			[]
[2]				[5,4,3]			[1]
[]				[5,4,3,2]		[1]
[]				[5,4,3,2,1]		[]


