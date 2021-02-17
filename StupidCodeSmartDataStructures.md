# Stupid Code, Smart Data Structures

### Summary:

If you model things right, it’s easy to work with them


### Details:

All your functions are small: 3-4 statements

Classes have 4-5 functions

Your classes contain no data, only logic

Functions accept only data structures (Arrays, trees, queues, stacks or hash tables)

All the primitives are encapsulated


### Success Criteria:



1. The code was much easier to write because of the way the data was structured.
2. You can create the board in any state easily, because you don’t need to manipulate the data through your methods.


### Example:

In the game below the goal is to select numbers one after the other (Player 1 is X, Player 2 is O)

Until one player gets 3 numbers that total 15.


<table>
  <tr>
   <td>1
   </td>
   <td>2
   </td>
   <td>3
   </td>
   <td>4
   </td>
   <td>5
   </td>
   <td>6
   </td>
   <td>7
   </td>
   <td>8
   </td>
   <td>9
   </td>
  </tr>
</table>


If you structure the board this way, it’s much easier to play:


<table>
  <tr>
   <td>8
   </td>
   <td>1
   </td>
   <td>6
   </td>
  </tr>
  <tr>
   <td>3
   </td>
   <td>5
   </td>
   <td>7
   </td>
  </tr>
  <tr>
   <td>4
   </td>
   <td>9
   </td>
   <td>2
   </td>
  </tr>
</table>

