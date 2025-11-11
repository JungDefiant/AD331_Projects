## Assignment: Generative AI with Pre-trained LLMs
Written by Bade Habib

### Model Used
distilgpt2 (based on GPT2)

### Chosen Task
Text Generation

### Test Cases
|Test Cases|Top-P|Max Tokens|Temperature|Output|Observation|
|---|---|---|---|---|---|
|1|0.9|50|0.6|"My favorite ice cream is iced with lemon juice. The ice cream is a bit more creamy, but the flavor is just a little bit sweeter. I have been wanting to try ice cream for a while now and I've been craving it for a while. I've"|Sounds human-like, but lacks understanding of what it's talking about.|
|2|0.9|50|0.2|"My favorite ice cream is iced cream. I love it, but I don't think I can get enough of it. I love it, but I don't think I can get enough of it. I love it, but I don't think I can get enough of it"|Repetitive and nonsensical.|
|3|0.6|50|0.6|"My favorite ice cream is iced cream. It’s not just a good idea to try it, but it’s also a great way to make your own ice cream."|Feels the most human-like, except for some inaccuracies in understanding context.|
|4|0.9|150|0.6|"My favorite ice cream is iced by Mottie, the sweet, sweet, and sweet flavors of ice cream."|Repetitive, somewhat whimsical, but doesn't make sense.|
