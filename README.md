# colab-demo

A Google Colab learning project for a university AI Agents course.

`creative_ideas.ipynb` asks for an everyday object and uses the OpenAI Responses API with `gpt-6-luna` to suggest exactly one unusual but practical use. The notebook includes simple English explanations and comments for beginners.

## Run in Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Choose **File → Upload notebook** and select the local `creative_ideas.ipynb` file, or [open the GitHub notebook directly in Colab](https://colab.research.google.com/github/nadeensuliman71-rgb/colab-demo/blob/main/creative_ideas.ipynb).
3. Connect to a Python 3 runtime and run each cell from top to bottom.
4. Let the first code cell install or update the OpenAI Python SDK.
5. Enter your OpenAI API key in the hidden `getpass` prompt. Your account needs access to `gpt-6-luna` and sufficient API credits; API usage may incur charges.
6. Enter an everyday object, such as a spoon, and run the final code cell to see the idea.

To try another object, rerun the object input cell and the generation cell. If a request fails, check your key, model access, API credits, and internet connection.

## Keep your API key private

Enter the key only in the hidden runtime prompt. Never paste it into source code, notebook text, outputs, or GitHub. The notebook keeps the key in runtime memory and does not write it to a file or print it. Clear notebook outputs before sharing, and delete the Colab runtime when finished.

The initial notebook is saved with no outputs. Its structure and code were checked locally, and it was successfully tested in Google Colab with "Umbrella" as input, generating one idea through the OpenAI Responses API without errors.
