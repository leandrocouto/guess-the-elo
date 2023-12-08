# Guess The Elo

Guess the Elo is a significant source of entertainment in online chess content. Content creators analyze entire chess games without knowledge of the players' ratings. They then attempt to guess the Elo based on various factors such as the players' ability to spot tricks, defend and attack effectively, and avoid blunders.

This project takes on the challenge of guessing a player's Elo based solely on a single chess position, introducing a higher level of difficulty compared to traditional Guess the Elo. The Convolutional Neural Network (CNN) used was trained using only the player's rating and chess positions; no additional information, such as an engine evaluation of the position, was provided.

The `data_collection` notebook outlines how the data was collected, while the `data_exploration` notebook discusses interesting insights gathered from the dataset. Finally, the `CNN` notebook details the preprocessing applied to the collected dataset, the training and validation processes. Toward the end of the notebook, results and the network's performance are thoroughly discussed, including considerations on potential improvements and insights for future projects based on this concept.

# Code Structure

    .
    ├── CNN.ipynb              # Preprocessing, Network implementation, Training and Discussion
    ├── README.md          
    ├── data_collection.ipynb  # Data collection using chess.com's public API       
    ├── data_exploration.ipynb # Analysis and visual inspection of the dataset
    ├── requirements.txt       # Dependencies necessary to run the notebooks
    └── trained_weights.keras  # Trained CNN model      

# Dependencies

`Python 3.8` was used for this project. You will need a Python environment that contains the packages listed in `requirements.txt`. 
You can create one with Python's built-in module `venv` running the following command:

```
python3 -m venv /path/to/project/guess-the-elo/venv/
```
After [activating](https://docs.python.org/3/library/venv.html) the virtual enviroment, you'll need to install the required packages:

```
python3 -m pip install -r requirements.txt
```

# License

Distributed under the MIT License.

```
Copyright (c) 2023 Leandro C. Medeiros

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

