
# Ranked 1st on the huggingface [Open Llm Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)   
This is a merged model. So you have to unckeck the "[X] Contains merge/moerge" checkbox above the list.   

## May 4th 2024 - avg. 81.28   
|             Metric              |Value|
|---------------------------------|----:|
|Avg.                             |81.28|
|ARC (25-Shot)                    |79.86|
|HellaSwag (10-Shot)              |91.32|
|MMLU (5-Shot)                    |78.00|
|TruthfulQA (0-shot)              |74.85|
|Winogrande (5-shot)              |87.77|
|GSM8k (5-shot)                   |75.89|

## Method
- I was inspired by this [Sakana project](https://sakana.ai/evolutionary-model-merge/)

## Process
This is a little bit tricky.
Anywany you need two models with the same architecture.
- Choose one model and fine-tune it to create a gap between the original model and the fine-tuned one. It doesn't matter whether the evaluation score is higher or lower.
- Merge the two models.
- Evaluate the merged model.
- Fine-tune a specific evaluation part of the model if you need to increase the score for that part. (It's unlikely to work as you think, but you can try it.)
- Merge the models again.
- Evaluate again.
- Keep going until the average evaluation score is higher than the original one.   

That's it. Simple.
You can create a framework to automate this process.

## Base Architecture 
- QWEN2

## Base Models
- several QWEN2 based models

<!--
**javafa/javafa** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
