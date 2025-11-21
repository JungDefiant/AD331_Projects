## Assignment: Prompt Engineering for Performance Improvement
Written by Bade Habib

### LLM & Embedding
- **LLM:** distilgpt2 (based on GPT2)
- **Embedding:** all-MiniLM-L6-v2

### Qualitative Analysis
|Prompt|Technique|Text|Score|
|---|---|---|---|
|1|Baseline|"Finish the following. DM: Galstaff, you enter the door to the north."|4|
|2|Role Prompting|"Pretend to be a Dungeon Master.\nFinish the following. DM: Galstaff, you enter the door to the north."|4|
|3|Output Formatting|"Use the following format. \nDM: <Describes what happens>\nPlayer: <Reacts to what happens>\nFinish the following. DM: Galstaff, you enter the door to the north."|3|
|4|One-Shot Prompting|"DM: You've been following this tunnel for about 120 yards... Finish the following using the prior example. DM: Galstaff, you enter the door to the north."|2|
|5|Final|"Pretend to be a Dungeon Master. DM: You've been following this tunnel for about 120 yards... Finish the following using the prior example. DM: Galstaff, you enter the door to the north."|5|

### Results Analysis
A combination of techniques doesn't necessarily ensure a result with more accuracy. The intricacies of how a prompt is written can also greatly affect the results. I found that an LLM can be pretty literal with instructions given or ignore instructions entirely. LLMs can also interpret a result as being part of a similar context as the one desired, but not exact. Overall, my results led to outputs that sounded "dream-like" and confused.
