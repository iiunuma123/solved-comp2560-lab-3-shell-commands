Download Link: https://assignmentchef.com/product/solved-comp2560-lab-3-shell-commands
<br>
Type the following into a file called <em>headandtail</em>:

Read the help pages for commands grep, cut, head, and tail.

When using grep with -n, each line of output is prefixed with a line number within its input file.

Check the output of the grep with line number.

When using cut, you can change the delimiter using -d.

Command head outputs the first part of files.

Check for the options for output the first n lines.

Command tail outputs the last part of files.

Part I – <em>head </em>and<em> tail</em>

Practice the following and understand the results.

head –n 5                                # type in at least 5 lines                                    head headandtail                                 head –n 2 headandtail                                      head –c 10                               # type “Joy to the world”

head –c 10 headandtail                                    tail –n 1 headandtail

head –n 5 headandtail | tail –n 2

Now use <em>pipe</em> to connect <em>head</em> and <em>tail</em> to print out the second and third lines of file <em>headandtail</em>.

Part II – <em>grep</em>

Type this command:

grep –n line &lt; headandtail

Check the print out and observe the line numbers separated by colons. Pipe this result with command <em>cut</em> to print out only the column of line numbers

Then pipe the above column of line numbers with command <em>head</em> to print out the first line number of the line containing word <em>line</em>.<em>  </em>

Part III

Use commands <em>grep</em>, <em>cut</em>, <em>head</em> and <em>tail</em> to write a bash script called <em>selector</em>. It accepts two words as arguments, and prints out the portion of the given file between the line of the first appearance of the first word (this line included) and the line of the first appearance of the second word (this line included).

You can assume that the first occurrence of the first word always appears earlier than the fist occurrence of the second word.

Sample run:

&gt;&gt;&gt;&gt;&gt; selector line delimiter

When using grep with -n, each line of output is prefixed with the 1-based line number within its input file.

Check the output of the grep with line number.

When using cut, you can change the delimiter using -d.

Part IV (optional)

Use bash <em>if</em>-statement and <em>test expression</em> to check if the first word appears after the second word. If so, inform the user about this.










2