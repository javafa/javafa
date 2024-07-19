
### May 4th 2024 - ranked 1st on the huggingface Open Llm Leaderboard
- This is a merged model. So you have to unckeck the "[X] Contains merge/moerge" checkbox above the list.

|             Metric              |Value|
|---------------------------------|----:|
|Avg.                             |81.28|

### free-evo-qwen72b-v0.8
- [model repository here](https://huggingface.co/freewheelin/free-evo-qwen72b-v0.8-re)   

### Method
- I was inspired by this [Sakana project](https://sakana.ai/evolutionary-model-merge/)

### Process
Required two models with the same architecture.   

1. Choose one model and fine-tune it to create a gap between the original model and the fine-tuned one. It doesn't matter whether the evaluation score is higher or lower.   
2. Merge the two models.   
3. Evaluate the merged model.   
4. Fine-tune a specific evaluation part of the model if you need to increase the score for that part. (It's unlikely to work as you think, but you can try it.)   
5. Merge the models again.   
6. Evaluate again.   
7. Continue until the average evaluation score is higher than the original one.   

### Base Architecture 
- QWEN2

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
