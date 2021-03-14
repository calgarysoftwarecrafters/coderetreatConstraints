# HexagonalGrid

### Summary:

Some cells feed off of their neighbors.

### Details:

1. If a cell has been alive longer than 100 cycles, it becomes a "Vampire Cell"

1. Vampire Cells do not count toward the neighbor count for live cell birth

1. Vampire Cells only conside other Vampire Cells when calculating their count for death, and the die when two or more Vampires are adjacent

1. Cells that would normally die but have a Vampire Cell adjacent to them, instead convert to a Vampire Cell



![image](images/vampire_cells.jpg)