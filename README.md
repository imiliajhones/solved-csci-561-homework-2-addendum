Download Link: https://assignmentchef.com/product/solved-csci-561-homework-2-addendum
<br>



Following discussion on Piazza about how to best prevent spoiling, the rules are updated as follows (see thread 334 and others on piazza):







<ol>

 <li><strong><u> Moving pieces</u> </strong></li>

 <li>Players cannot make a move that starts outside their own camp and causes one of their pieces to end up in their own camp.</li>

</ol>




<ol>

 <li>If a player has at least one piece left in their own camp, they have to

  <ul>

   <li>Move a piece out of their camp (i.e. at the end of the whole move the piece ends up outside of their camp).</li>

   <li>If that’s not possible, move a piece in their camp further away from the corner of their own camp ([0,0] or [15,15] respectively).</li>

  </ul></li>

</ol>




Only if the player does not have any pieces left in their camp or none of the two alternatives above are possible are they free to move pieces outside of their camp.




Note: To move “further away”, you should simply move so that you either move further away horizontally (while not moving closer vertically), or vertically (while not moving closer horizontally), or both.







<ol start="2">

 <li><strong><u> Winning the game (no real change here, just a clarification)</u> </strong></li>

</ol>

A player wins if they are the first to fill out all the space in the opposite camp that’s not occupied by the opposite player’s pieces using at least one of their pieces.




<strong><u>What you should do:</u> </strong>




If you already have some code that plays according to the original rules, likely somewhere you have a function that lists or loops over all the moves that your agent could take given the current state of the board. You should modify this function slightly to remove the possible moves that would violate the new rules above. We expect that no change should be necessary to your core minimax and alpha-beta code, although this may depend on your exact implementation.





