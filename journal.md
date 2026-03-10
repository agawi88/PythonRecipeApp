# Learning Journal

## March 10, 2026
### Topic No. 1: Python environments and pip

What I learned:
- How to activate a virtual environment
- How to install packages with pip
- How to generate requirements.txt

Challenges:
- I mistakenly tried to run pip commands inside the Python REPL as well as outside the environment.

Solution:
- Ran pip install commands in the terminal instead.

Key takeaway:
Terminal commands and Python code run in different places.

### Topic No. 2: Git commits and pushing files to GitHub

What I learned:
Today I learned how staging files works in Git when committing and pushing changes to a GitHub repository via the code proivided on gitHub.

Challenge:
After creating my repository and pushing the project, only the `README.md` file appeared on GitHub even though my project folder also contained `add.py` and `requirements.txt`.

Cause:
I realized that I had used the command `git add README.md`, which only staged that single file for the commit. Because the other files were never staged, they were not included in the commit and therefore not pushed to GitHub.

Solution:
To fix the issue, I staged the missing files and committed them:

git add add.py requirements.txt  
git commit -m "Add project files"  
git push

Key takeaway:
Git only commits files that have been explicitly staged. Using `git add .` is often easier because it stages all new and modified files in the project directory.


### Topic No. 3: Difference between REPL testing and writing Python scripts

What I learned:
During this exercise I learned the difference between testing code in the Python REPL/IPython and writing a program in a Python file. The REPL is an interactive environment where commands can be tested quickly, while a `.py` file contains a script that runs when executed from the terminal.

Challenge:
I was initially confused about where to write the code for adding two numbers. I tried to type the program logic in the REPL and wasn't sure whether it should instead go into the `add.py` file.

Resolution:
I learned that the REPL is mainly used to experiment with small pieces of code, while the actual program should be written in a `.py` file and then run from the terminal using `python add.py`.

Key takeaway:
The REPL is useful for testing ideas quickly, but Python programs are typically written in script files that are executed from the terminal.