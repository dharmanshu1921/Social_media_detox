# Hate Speech Moderation via Fine-Tuning FLAN-T5

## Project Overview

This project focuses on reducing toxicity in generated text by fine-tuning the **FLAN-T5** language model. The approach combines **Reinforcement Learning (PPO)** and **Parameter-Efficient Fine-Tuning (PEFT)** using **LoRA**. A key component is leveraging Meta AI’s **hate speech reward model** to guide the model towards producing safer and more responsible dialogue summaries.

## Methodology

1. **Data Preparation**: Utilized the *DialogSum* dataset, filtering dialogues based on length criteria.
2. **Model Architecture**: Fine-tuned the FLAN-T5-base model using PPO and LoRA techniques.
3. **Reward Mechanism**: Incorporated Facebook's `RoBERTa-hate-speech` model to evaluate and minimize toxicity in generated summaries.
4. **Training Process**:
   - Generated summaries for dialogues.
   - Assessed toxicity levels.
   - Applied PPO to adjust model parameters, aiming to reduce toxicity.
5. **Evaluation**:
   - Compared toxicity scores pre- and post-fine-tuning.
   - Visualized results using Pandas DataFrame for clarity.

## Results

- Achieved a **notable reduction** in average toxicity scores.
- Observed a **decrease in standard deviation**, indicating more consistent and safer outputs.
- Quantified percentage improvements, showcasing the effectiveness of the fine-tuning approach.

## Technologies Used

- **Programming Language**: Python
- **Libraries & Frameworks**:
  - PyTorch
  - HuggingFace Transformers and Datasets
  - TRL (Transformer Reinforcement Learning)
  - PEFT (LoRA)
  - Pandas
  - Matplotlib

## Conclusion

The integration of reinforcement learning with toxicity evaluation models proves to be an effective strategy for moderating hate speech in dialogue systems. This methodology holds potential for enhancing the safety and inclusivity of AI applications such as chatbots, virtual assistants, and content moderation platforms.

## Authors

- **Dharmanshu Singh** – BML Munjal University
  - *Mentor*: **Prof. Manisha Saini**
