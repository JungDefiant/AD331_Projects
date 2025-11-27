## Milestone 3: MVP

### Model & Dataset
**Model:** bert-base-cased
**Dataset:** imdb

### LoRA Config
**Task Type:** Sequence Classification
**R:** 8
**Alpha:** 32
**Dropout:** 0.1

### Evaluation
**Loss:** ~0.6177
**Accuracy:** 68.8%
**Runtime:** 186.6918 seconds
**Epochs:** 5

### Follow-Up
**Why does LoRA save resources?**
Historically, fine-tuning models involved retraining the entire model to be better suited for a particular task. With the LoRA technique, only a small number of weights relevant to the context are injected into the model, which greatly reduces the number of parameters trained. Think of a painting that an artist has worked on for weeks and wants to make changes. Rather than remaking the entire painting, the artist can modify the painting to better suit their vision. This is how LoRA works in regards to fine-tuning models.
