\definecolor{DarkGreen}{HTML}{008000}

# Feedback

## Exercise 1

\color{DarkGreen}

I think you fundamentally misunderstood the exercise, since you only provided specific values for the weights/biases and not how to set them for an arbitrary vertex (at least it seems like it) so I can't really write any feedback on how to fix this.

The rest of the exercise (sketch, classification, hypercube) is missing.

\color{black}

## Exercise 2

\color{DarkGreen}

Compared to the author's solution, it doesn't consume the biases but instead multiplies two layers into one, which is also correct (we can repeat this until we merge all layers).

\color{black}

## Exercise 3
Team provided the `.html` and the `.ipynb` files, but they are not actually that -- both are just a Python script that combines all the cells into one file.
If this is intentional, **PLEASE DO NOT DO IT THIS WAY IN THE FUTURE** since it is extremely confusing (the filetypes should **ALWAYS** correspond to their contents) and greatly complicates the feedback (I have to run the code to confirm that it works and also can't easily comment the appropriate sections).

\color{DarkGreen}

### ReLULayer

- forward: same
- backward: seems wrong, sign should be used instead (if you want to use self.input like this)

### OutputLayer

- forward: correct but doesn't subtract maximum so is numerically less stable
- backward: same

### LinearLayer

- forward: same
- backward: same

### MLP

- backward: same

Running the code seems to yield correct results, however (the incorrect backward derivation of ReLU is pretty close to the correct one).

\color{black}
