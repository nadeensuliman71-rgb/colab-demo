# colab-demo

A Google Colab learning project for a university AI Agents course.

`creative_ideas.ipynb` uses the OpenAI Responses API with `gpt-6-luna` to suggest three unusual, practical, and different uses for an everyday object. It displays the ideas as a numbered list (1, 2, 3).

A simple Python `while` loop lets you enter objects repeatedly without restarting the notebook. Type `quit` or `exit` to stop. Blank input shows a reminder without making an API request. Failed requests and unexpected response formats show a friendly message and let you try again. The notebook includes simple English explanations and comments for beginners.

## Run in Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. [Open the notebook directly in Colab](https://colab.research.google.com/github/nadeensuliman71-rgb/colab-demo/blob/main/creative_ideas.ipynb), or choose **File → Upload notebook** and select the local `creative_ideas.ipynb` file.
3. Connect to a Python 3 runtime and run each cell from top to bottom.
4. Let the first code cell install or update the OpenAI Python SDK.
5. Enter your OpenAI API key in the hidden `getpass` prompt. Your account needs access to `gpt-6-luna` and sufficient API credits; API usage may incur charges.
6. Run the generator cell in step 3. Enter an everyday object, such as a spoon, at its prompt to see three numbered ideas.
7. Enter another object when prompted. Keep using the same running cell, and type `quit` or `exit` when finished. Stop words are case-insensitive and surrounding spaces are ignored.

Each object sends a separate API request. If a request fails, check your key, model access, API credits, and internet connection, then enter the object again. If you need to replace the key, stop the loop, rerun the key-entry cell, and rerun the generator cell. After quitting, you can also rerun the generator cell to start again.

## Test the final version

In one run, try at least three different objects, such as **Umbrella**, **Spoon**, and **Cardboard box**. For each object, check that there are exactly three numbered uses and that they are unusual, practical, and different in meaning. The code checks the count, numbering, and identical text; the model is responsible for the ideas' quality and variety.

Also submit an empty input to check the reminder, then type `quit` to check stopping. Rerun the generator cell and try `exit` too. The program should keep asking after blank input or a failed API request.

## Keep your API key private

Enter the key only in the hidden runtime prompt. Never paste it into source code, notebook text, outputs, or GitHub. The notebook keeps the key in runtime memory and does not write it to a file or print it. Clear notebook outputs before sharing, and delete the Colab runtime when finished.

The notebook is saved with no outputs. The final version was successfully tested in Google Colab with **Umbrella**, **Spoon**, and **Cardboard box** in one run. Each object produced three numbered practical ideas, and typing `quit` stopped the program. Local structure, syntax, and simulated control-flow checks also passed. The Git history preserves the initial one-idea version and the final version with three ideas and repeated input.
