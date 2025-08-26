Hi! Let's do some mechanistic interpretability! I've created and activated a fresh conda environment in the current directory, 'llm-not-assistant'.

Taking inspiration from the techniques and idioms used in the Google Colab notebook in this directory (/Users/egg/Documents/Programming/llm-not-assistant/1_2_Intro_to_Mech_Interp_solutions.ipynb — you don't have to read the whole thing, just look at some of it, especially the early parts), I'd like you to put together a Colab notebook / Jupyter notebook based on TransformerLens which does the following:
* Loads in an instruction-tuned LLM supported by TransformerLens (by default, use some very small model that's easy to run locally).
* Identifies that model's typical template (probably looking something like `<|im_start|>user: [prompt]<|im_end|>\n<|im_start|>assistant: `).
  * Note: I'm not sure whether these templates are included with the model in TransformerLens? Please check to see how this is usually handled and let me know.
* Remove the `assistant: ` (or equivalent) part of the template and test with a few typical prompts (eg 'Hi!', 'What is the tallest building in the world?', 'What is 7 + 9?').
* Show how strongly the model then predicts the `assistant` token.
* (start a new section)
* Ablate the `assistant` token, and sample (and print) 10 completions from the model at temperature=0.3 (or equivalent via top-k / top-p).

What do you think? Does everything there seem reasonably straightforward and doable? What if anything have I failed to specify? What else do you need to know?

