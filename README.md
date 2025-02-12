# wordle
A simple Python notebook that imitates [wordle](https://www.nytimes.com/games/wordle/index.html)!

If you're not familiar with it, wordle is basically a "guess the word" game. You have 6 tries to attempt to guess a letter word. For each guess, it will give feedback in the form of colored tiles indicating when letters match or occupy the correct position: 
- Green for when you get the letter on the right position
- Yellow for when the letter is in the word but in another position
- Gray if the letter is not in the word.

## How to play  
In this repo, you will find a very simple prototype of the game in the Jupyter notebook called `wordle.ipynb`. I suggest you try playing it on VS Code, either on the web or the Desktop. You will find the set up steps below. 

### Web set up
 To play it on the web, simply open this repo in [vscode.dev](https://vscode.dev/), or  just press "." if you're reading this on GitHub to open it in [github.dev](https://github.dev/).
 Open the Extensions view (`Ctrl + Shift + X` or `Cmd + Shift + X`) and look for the "vscode-pyodide" extension, published by "joyceerhl". Go ahead and install it.

### Desktop set up
[Download VS Code](https://code.visualstudio.com/) and install the following extensions:
- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
- [Jupyter Notebooks](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)

Then open this repo in VS Code, and open the `wordle.ipynb` file.  

If you don't have Python installed, you can follow the steps [here](https://code.visualstudio.com/docs/python/python-tutorial#_install-a-python-interpreter). When you try to run the first cell in the notebook, you will be able to follow  some set up steps to get your environment ready to use the notebook features. 

### Placing your guess

Once you're able to run the first cell, you can place your first guess by creating a new cell (Ctrl + Enter or ⌘ + Enter) and calling the `guess_word` function and passing a string with your first word to it. For example, you can try `guess_word("ghost")`.


For each guess you make, you will get:
- `_` if you got the letter on the right position
- `*` if the letter is in the answer word but in another position
- The letter itself when you get it in the right position.

If you get the word right with 6 or less guesses, you win the game. If you don't, you lose.

To play again, simply re-run the first cell and it will reset the turns and pick a different word for you. 

![Running cells by calling guess_word(string)to play the game.](https://github.com/luabud/wordle/blob/main/images/example.png?raw=true)
 


