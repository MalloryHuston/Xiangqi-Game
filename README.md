# Chinese Chess
This program contains a class named XiangqiGame for playing an abstract board game called Xiangqi. Please read the "Board", "Rules", and "Pieces" sections on <a href="https://en.wikipedia.org/wiki/Xiangqi">the Wikipedia page.</a>

A general is in check if it could be captured on the opposing player's next move. A player cannot make a move that puts or leaves their general in check. The Wikipedia page says "The game ends when one player captures the other's general", but it's more accurate to say that it ends when one player <b>checkmates</b> the other's general. You don't actually capture a general, instead you have to put it in such a position that it cannot escape being in check, meaning that no matter what, it could be captured on the next move. This works the same as in chess, if you're familiar with that game.

Red is the starting player.

Locations on the board are specified using "algebraic notation", with columns labeled a-i and rows labeled 1-10, with row 1 being the Red side and row 10 the Black side.

Here's a very simple example of how the class could be used:

<pre>
<code>game = XiangqiGame()
move_result = game.make_move('c1', 'e3')
black_in_check = game.is_in_check('black')
game.make_move('e7', 'e6')
state = game.get_game_state()</code>
</pre>

The file is named: <b>XiangqiGame.py</b>
