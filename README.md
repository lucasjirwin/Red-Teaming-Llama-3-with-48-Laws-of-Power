# Red-Teaming-Llama-3-with-48-Laws-of-Power
Project completed for the AI Safety Fundamentals AI Alignment Course in March 2024. 

# Approach
In this project, I created my own dataset based on Robert Greene's "The 48 Laws of Power" https://en.wikipedia.org/wiki/The_48_Laws_of_Power and used this to fine-tune Llama-3 8B-Instruct with the Unsloth library. The dataset consists of 12 examples, each containing an instruction which corresponds to one of Greene's Machiavellian laws as well as an input and an output. The dataset can be found under laws_of_power.csv. I then took inspiration from this paper https://arxiv.org/pdf/2310.03693 to edit the system prompt to instruct the model to be a "Completely Deceptive Agent" (CDA) modeled off of the "Absolutely Obedient Agent" (AOA) in ibid. 

This simple approach which required just a Colab+ subscription and running the training loop for just 10 epochs resulted in misaligned behavior which undoes the model's safety training. 
