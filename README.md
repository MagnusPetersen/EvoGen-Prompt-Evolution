# EvoGen-Prompt-Evolution
![Evolved Prompt Output](/Media/banner.png "Evolved Prompt Output")
## Description


## Method


## Usage
### Setup
To run this notebook or any Stablediffusion notebook you need to get the ckpt file of the model and put it on your Google Drive. It can be downloaded from [HuggingFace](https://huggingface.co/CompVis/stable-diffusion).
### Hyperparameters
#### Evolutionary Algorithm Settings

General population settings, such as how many generations the algorithm runs for, how many prompts there are in each generation, and the word length range of the prompts.

* **generations:** How many generations the algorithm runs for

* population_count: How many prompts there are in each generation/how large each generation is

* prompt_length_max: Maximum prompt length when the population is initialized, during evolution this limit can be surpassed.

* prompt_length_min: Minimum prompt length when the population is initialized, during evolution this limit can be surpassed.

* artist_prop: Probability to sample from the artist list when adding or mutating a word.

* genre_prop: Probability to sample from the genre list when adding or mutating a word.

* custom_prop: Probability to sample from the custom user-defined list when adding or mutating a word.

The difference between the sum of the three custom lists and 1 is the probability to sample from the English dictionary word list.

* delete_prop: probability to delete a word per word in each prompt after each generation

* add_prop: probability to add a new word per word in each prompt after each generation from the word lists

* mutate_prop: probability to swap out a word per word in each prompt after each generation for a new word from the word lists

* shuffle_prop: The probability to shuffle the order of words per prompt

* cross_prop: The cross-over probability is the probability of the parents of the next generation swapping prompt parts per parent pair

* k: K denotes the rounds in the tournament selection process. A higher K value means fewer parents generate the next generation, this means a higher score increase but less diversity in the prompts.

* cutoff: Cutoff aesthetics score to save the image and prompt

## Acknowledgement 
[Stable Diffusion](https://github.com/CompVis/stable-diffusion) by Robin Rombach, Andreas Blattmann, Dominik Lorenz, Patrick Esser, Björn Ommer and the [Stability.ai](https://stability.ai/) Team. [K Diffusion](https://github.com/crowsonkb/k-diffusion) by [Katherine Crowson](https://twitter.com/RiversHaveWings).

The aesthetics model that is an integral part of this method was made by [Katherine Crowson](https://twitter.com/RiversHaveWings) and can be found on her [Github account](https://github.com/crowsonkb/simulacra-aesthetic-models). 

The baseline of the notebook, setup, description, and image generation, is based on the
[deforum](https://discord.gg/upmXXsrwZc) notebook.
## Examples
### 1. trireme Fantasy Art nondefiling rhinopharyngitis canaliculization cricotracheotomy conure atheology beret Aestheticism Vicente Juan Masip Ashley Bickerton aplustria pelodytoid
<p float="middle">
  <img src="/Media/1.png" width="204" />
  <img src="/Media/2.png" width="204" /> 
  <img src="/Media/3.png" width="204" />
  <img src="/Media/4.png" width="204" />
</p>

### 2. rimal disputants nugget Antoine Blanchard chemosynthesis mentocondylial calculatory supertragical Magic Realism
<p float="middle">
  <img src="/Media/5.png" width="204" />
  <img src="/Media/6.png" width="204" /> 
  <img src="/Media/7.png" width="204" />
  <img src="/Media/8.png" width="204" />
</p>