<h3>Project name:</h3>
<h2> pipex</h2>

<b>Project description:</b>
This project aims to make understand a bit deeper two concepts that already know: the redirections and the pipes.

<b>Task:</b>
<p>Your program will be executed as follows:</p>
<p>./pipex file1 cmd1 cmd2 file2</p>
<p>It must take 4 arguments:</p>
<p>• file1 and file2 are file names.</p>
<p>• cmd1 and cmd2 are shell commands with their parameters.</p>
<p>It must behave exactly the same as the shell command below:</p>
<p>$> < file1 cmd1 | cmd2 > file2</p>
  
<p>Examples</p>
<p>$> ./pipex infile "ls -l" "wc -l" outfile</p>
<p>Should behave like: < infile ls -l | wc -l > outfile</p>
<p>$> ./pipex infile "grep a1" "wc -w" outfile</p>
<p>Should behave like: < infile grep a1 | wc -w > outfile</p>
<p>Your project must comply with the following rules:</p>
<p>• You have to turn in a Makefile which will compile your source files. It must not relink.</p>
<p>• You have to handle errors thoroughly. In no way your program should quit unexpectedly (segmentation fault, bus error, double free, and so forth).</p>
<p>• Your program mustn’t have memory leaks.</p>
<p>• If you have any doubt, handle the errors like the shell command:</p>
<p>< file1 cmd1 | cmd2 > file2</p>

