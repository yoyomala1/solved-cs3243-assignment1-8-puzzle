Download Link: https://assignmentchef.com/product/solved-cs3243-assignment1-8-puzzle
<br>
In this assignment, you will be implementing two different search algorithms of your choosing on the 8-puzzle game introduced in the lecture. At the end of this assignment, you should be able to identify and comment on the difference in performance of the algorithms.

<h2>2      Background</h2>

The 8-puzzle is a sliding puzzle that consists of a frame of numbered square tiles in random order with one tile missing. The objective of the puzzle is to arrange the tiles in order by making sliding moves that use the empty space. Figure 1 shows a sample initial state for 8-puzzle.

Figure 1: A sample initial state

<h2>3       Problem Statement</h2>

An initial state will be given as input. Your job is to solve the puzzle to reach the goal state (see Figure 2) and output the <strong>actions</strong>. Notice that some initial states may not be solvable. For example, Figure 3 shows an unsolvable initial state. In this case, you only need to output <strong>UNSOLVABLE</strong>.

<h3>3.1     Input</h3>

The input will be provided in a text file containing three lines to represent the initial state. Each line contains three numbers. They must include the numbers 0–8, where 0 represents the empty space, and 1–8 represents the 8 tiles of the puzzle. For example, the initial state in Figure 1 is encoded in the text file as follows:

0 1 3

4 2 5

7 8 6

<h3>3.2     Output</h3>

<ul>

 <li>Your output should be written to a file in the form of a <strong>List</strong>. If the initial state is Figure 1, one possible output could be <strong>[“LEFT”, “UP”, “LEFT”, “UP”]</strong>. This will be stored in the file as shown below.</li>

</ul>

[‘‘LEFT’’, ‘‘UP’’, ‘‘LEFT’’, ‘‘UP’’]

<ul>

 <li>If the input puzzle is not solvable, output <strong>[“UNSOLVABLE”]</strong>. Otherwise, output the action of each step. The action could only be <strong>“UP”</strong>, <strong>“DOWN”</strong>, <strong>“LEFT”</strong>, <strong>“RIGHT”</strong>, to represent the direction of moving the tile towards the space.</li>

 <li>You should ensure each action is valid (e.g., you <strong>CANNOT </strong>move <strong>DOWN </strong>when the space is in the first line) and the puzzle should be the same to the goal state after the last action.</li>

</ul>