
# Generative AI with Large Language Models (LLMs)

This folder contains notebooks, summaries and notes for the course [Generative AI with LLMs](https://www.coursera.org/learn/generative-ai-with-llms) accesible on Coursera. The notebooks are all notebooks of the course. The solutions are my own work. All the rest has been created by [deeplearning.ai](https://www.deeplearning.ai/) in collaboration with [AWS](https://aws.amazon.com/) and thus, the credit goes to

```
Coursera
deeplearning.ai
AWS
```

The learning objectives of each week are stated as follows 

<table>
  <tr>
    <th>Week</th>
    <th>Learning Objectives</th>
    <th>Lab</th>
    <th>Resources</th>
    <th>Quizzes</th>
  </tr>
  <tr>
    <td>1️⃣</td>
    <td>
      <ul>
        <li>Generative AI use cases, project lifecycle, and model pre-training</li>
      </ul>
    </td>
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/525f7711b8d25af49dedd3b13041a7ab0053f484/courses/generative_ai_with_llms/Lab_1_summarize_dialogue.ipynb">Lab 1</a></td>    
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/generative_ai_with_llms/courses/generative_ai_with_llms/resources.md">Resources</a></td>
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/generative_ai_with_llms/courses/generative_ai_with_llms/quizzes.md">Quizzes</a></td> 
  </tr>
  <tr>
    <td>2️⃣</td>
    <td>
      <ul>
        <li>Describe how fine-tuning with instructions using prompt datasets can improve performance on one or more tasks</li>
        <li>Define catastrophic forgetting and explain techniques that can be used to overcome it</li>
        <li>Define the term Parameter-efficient Fine Tuning (PEFT)</li>
        <li>Explain how PEFT decreases computational cost and overcomes catastrophic forgetting</li>
        <li>Explain how fine-tuning with instructions using prompt datasets can increase LLM performance on one or more tasks</li>
      </ul>
    </td>
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/4d3fb3985f78f6c5f3d94f821ccaa625ccbb15b0/courses/generative_ai_with_llms/Lab_2_fine_tune_generative_ai_model.ipynb">Lab 2</a></td>    
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/generative_ai_with_llms/courses/generative_ai_with_llms/resources.md">Resources</a></td>
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/generative_ai_with_llms/courses/generative_ai_with_llms/quizzes.md">Quizzes</a></td>     
  </tr>
  <tr>
    <td>3️⃣</td>
    <td>
      <ul>
        <li>Describe how RLHF uses human feedback to improve the performance and alignment of large language models</li>
        <li>Explain how data gathered from human labelers is used to train a reward model for RLHF</li>
        <li>Define chain-of-thought prompting and describe how it can be used to improve LLMs reasoning and planning abilities</li>
        <li>Discuss the challenges that LLMs face with knowledge cut-offs, and explain how information retrieval and augmentation techniques can overcome these challenges</li>
      </ul>
    </td>
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/c6c4e2770585b11f59a257b1ca59422728f30149/courses/generative_ai_with_llms/Lab_3_fine_tune_model_to_detoxify_summaries.ipynb">Lab 3</a></td>    
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/generative_ai_with_llms/courses/generative_ai_with_llms/resources.md">Resources</a></td>
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/generative_ai_with_llms/courses/generative_ai_with_llms/quizzes.md">Quizzes</a></td>    
  </tr>
</table>

## Notes 

Instead of downloading from S3 one can also directly copy the S3 content from a AWS SageMaker terminal. 

```bash
aws s3 cp --recursive s3://dlai-generative-ai/labs/w1-549876/ ./
```


