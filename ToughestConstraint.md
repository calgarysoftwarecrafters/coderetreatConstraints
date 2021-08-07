# The Toughest Constraint (So far...)

### Summary
So, you're _really_ up for a challenge, eh?

### Description
This constraint comes from [this blog article by Adrian Bolboaca](https://blog.adrianbolboaca.ro/2014/11/coderetreat-toughest-constraint/). It mixes the Hexagonal board constraint with wormholes, a dynamic space structure, and a flexible definition of time. Still want to give it a go? Read on.

#### 1. Start with an orthogonal board
Conway's normal rules apply here.

#### 2. Add Wormholes
A wormhole is a vertical band of cells that sends cells from one place to another on an orthogonal board.
1. The number, width, location, output, and duration of each wormhole is determined randomly at the beginning of each turn
2. Each wormhole has two bands of pentagonal space at it's entrance and exit. These bands bridge the orthogonal space outside of the wormhole with the hexagonal space within.

#### 3. The Hexagonal space inside the wormhole
Each cell has 6 first-tier neighbours (The ones immediately surrounding it) and 6 second-tier neighbours:

```
_ _ _ _ _ _ _ _
 _ _ _ 2 _ _ _ 
_ _ 2 1 1 2 _ _
 _ _ 1 X 1 _ _ 
_ _ 2 1 1 2 _ _
 _ _ _ 2 _ _ _ 
_ _ _ _ _ _ _ _
```

When calculating whether or not a cell should survive, first tier neighbours add 1 point to the cell's survivability score. Secont tier neighbours add 0.3 points.
* A live cell with a survivability score less than 2.0 dies
* A live cell with a survivability score between 2.0 and 3.3 survives
* A live cell with a survivability score more than 3.3 dies
* A dead cell with a survivability score between 2.3 and 2.9 lives

#### 4. Time is not constant
If you have one tick in the orthogonal space, in the pentagonal gate (the transient area) you have that 1 tick equivalent to 7.6. When you pass into the hexagonal space, the 1 tick is equivalent to 0.72.
