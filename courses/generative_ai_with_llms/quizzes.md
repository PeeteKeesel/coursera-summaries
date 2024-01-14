This page contains all the quizzes from the course. 

# Week :one: 

1. Interacting with Large Language Models (LLMs) differs from traditional machine learning models.  Working with LLMs involves natural language input, known as a `___`, resulting in output from the Large Language Model, known as the `___`. Choose the answer that correctly fill in the blanks.
- [ ] prompt, fine-tuned LLM
- [ ] prediction request, prediction response
- [ ] tunable request, completion
- [x] prompt, completion
  - > The input for working with LLMs is referred to as the prompt and the output from the LLM is referred to as the completion.
2. Large Language Models (LLMs) are capable of performing multiple tasks supporting a variety of use cases.  Which of the following tasks supports the use case of converting code comments into executable code?
   - [ ] Information Retrieval
   - [ ] Text summarization
   - [x] Translation
     - > Translation focuses on converting languages, including coding languages so in this case the task focuses on translating code comments into executable code.
   - [ ] Invoke actions from text
3. What is the _self-attention_ that powers the transformer architecture?
   - [ ] The ability of the transformer to analze its own performance and make adjustments accordingly.
   - [ ] A technique used to improve the generalization capabilities of a model by training it on diverse datasets.
   - [x] A mechanism that allows a model to focus on different parts of the input sequence during computation.
     - > Self-attention is a key component in models like Transformers, where it enables the model to attend to different words in the input sequence to capture their relationships and dependencies.
   - [ ] A measure of how well a model can understand and generate human-like language.
4. Which of the following stages are part of the generative AI model lifecycle mentioned in the course? (Select all that apply)
   - [x] Defining the problem and identifying relevant datasets.
     - > It is crucial to define the problem being solved and identify relevant datasets instrumental to the project.
   - [x] Selecting a candidate model and protentially pre-training a custom model.
     - > Selecting a candidate model and potentially pre-training a custom model are important stages in the generative AI model lifecycle.
   - [x] Deploying the model into the infrastructure and integrating it with the application.
     - > Once we have a model performing to our needs, we can deploy it into the infrastructure and integrate it with the application.
   - [ ] Performing regularization
   - [x] Manupulating the model to align with specific project needs.
     - > It is likely we will have to manipulate the model in some way to align it with the specific needs of the project.
5. "RNNs are better than Transformers for generative AI Tasks.". Is it True or False? 
   - [ ] True
   - [x] False
     - > While RNNs can be used for generative AI tasks, they struggle with compute and memory, making it hard to keep context in longer texts. The transformers architecture is more parallelizable and its dynamic attention mechanism helps to capture long-range dependencies in the input.
6. Which transformer-based model architecture has the objective of guessing a masked token based on the previous sequence of tokens by building bidirectional representations of the input sequence.
   - [ ] Sequence-to-sequence
   - [x] Autoencoder
     - > Autoencoder models are pre-trained using masked language modeling.  They use randomly masked tokens in the input sequence and the pretraining objective is to predict the masked tokens to reconstruct the original sentence. 
   - [ ] Autoregressive
7. Which transformer-based model architecture is well-suited to the task of text translation?
   - [x] Sequence-to-sequence
     - > Sequence-to-sequence models use both the encoder and decoders in the transformer-based architecture making them best suited for tasks such as translation, text summarization, and question answering. In the Transformers video, Mike explains it in more detail.
   - [ ] Autoencoder
   - [ ] Autoregressive
8. Do we always need to increase the model size to improve its performance?
Is it True or False? 
   - [ ] True
   - [x] False
     - > Recent trends show that we can build better LLMs without necessarily increasing model size year by year. Models like LLaMa and BloombergGPT have demonstrated the possibility of reducing model size while keeping great performance.
9.  Scaling laws for pre-training large language models consider several aspects to maximize performance of a model within a set of constraints and available scaling choices.  Select all alternatives that should be considered for scaling when performing model pre-training?
    - [x] Dataset size: Number of tokens
      - > The size of the pre-training data is an important factor to consider when scaling with compute constraints. This is because the size of the dataset directly affects the computational requirements during pre-training, and having a larger dataset generally leads to improved model performance.
    - [x] Model size: Number of parameters
      - > The size of the model in terms of number of parameters is a key scaling choice to consider with compute constraints because the number of parameters directly impacts the compute needs required during pre-training. 
    - [ ] Batch size: Number of samples per iteration
    - [x] Compute budget: Compute constraints
      - > The compute budget plays a crucial role in scaling during pre-training. When faced with a limited compute budget, we may need to impose restrictions on either the model size or the dataset size.
10. "You can combine data parallelism with model parallelism to train LLMs." Is it True or False?   
    - [x] True
      - > Combining data parallelism with pipeline parallelism is known as 2D parallelism.We can achieve 3D parallelism by combining data parallelism with both pipeline parallelism and tensor parallelism simultaneously.
    - [ ] False


# Week :two: 

1. Fill in the blanks: `___` involves using many prompt-completion examples as the labeled training dataset to continue training the model by updating its weights. This is different from `___` where you provide prompt-completion examples during inference.
- [x] Instruction fine-tuning, In-context learning
- [ ] In-context learning, Instruction fine-tuning
- [ ] Prompt engineering, Pre-training
- [ ] Pre-training, Instruction fine-tuning
2. Fine-tuning a model on a single task can improve model performance specifically on that task; however, it can also degrade the performance of other tasks as a side effect.  This phenomenon is known as: 
- [ ] Instruction bias
- [ ] Model toxicity
- [ ] Catastrophic loss
- [x] Catastrophic forgetting
3. Which evaluation metric below focuses on precision in matching generated output to the reference text and is used for text translation?
- [ ] HELM
- [ ] ROUGE-2
- [ ] ROUGE-1 
- [x] BLEU
  - > BLEU focuses on precision and text translation while Rouge focuses on text summarization.
4. Which of the following statements about multi-task finetuning is correct? Select all that apply:
- [ ] Performing multi-taks finetuning may lead to slower inference.
- [x] Multi-task finetuning can help prevent catastrophic forgetting.
  - > Correct! However, remember that to prevent catastrophic forgetting it is important to fine-tune on multiple tasks with a lot of data.
- [ ] Multi-task finetuning requires separate models for each task being performed.
- [x] FLAN-T5 was trained with multi-taks finetuning.
  - > The FLAN family of models have been trained with multi-task instruction finetuning.
5. "Smaller LLMs can struggle with one-shot and few-shot inference:"
- [x] True
  - > Even when you include a couple of examples, smaller models might still struggle to learn the new task through examples.
- [ ] False
6. Which of the following are Parameter Efficient Fine-Tuning (PEFT) methods? Select all that apply.
- [x] Selective
  - > Selective methods is a category of PEFT that fine-tunes a subset of the original LLM parameters. It uses different approaches to identify which parameters to update.
- [x] Additive
  - > Additive methods freeze all of the original LLM weights and introduce new model components to fine-tune to a specific task. 
- [ ] Subtractive
- [x] Reparameterization
  - > Reparameterization methods create a new low-rank transformation of the original network weights to train, decreasing the trainable parameter count while still working with high-dimensional matrices. LoRa is a common technique in this category.
7. Which of the following best describes how LoRA works?
- [ ] LoRA continues the original pre-training objective on new data to update the weights of the original model.
- [x] LoRA decomposes the weights into two smaller rank matrices and trains those instead of the full model weights.
  - > LoRA represents large weight matrices as two smaller, rank decomposition matrices, and trains those instead of the full weights. The product of these smaller matrices is then added to the original weights for inference.
- [ ] LoRA trains a smaller, distilled version of the pre-trained LLM to reduce model size.
- [ ] LoRA freezes all weights in the original model layers and introduces new components which are trained on new data.
8. What is a soft prompt in the context of LLMs (Large Language Models)?
- [x] A set of trainable tokens that are added to a prompt and whose values are updated during additional training to improve performance on specific tasks.
  - > A soft prompt refers to aa set of trainable tokens that are added to a prompt. Unlike the tokens that represent language, these tokens can take on any value within the embedding space. The token values may not be interpretable by humans, but are located in the embedding space close to words related to the language prompt or task to be completed.
- [ ] A strict and explicit input text that serves as a starting point for the model's generation.
- [ ] A technique to limit the creativity of the model and enforce specific output patterns.
- [ ] A method to control the model's behavior by adjusting the learning rate during training.
9.  "Prompt Tuning is a technique used to adjust all hyperparameters of a language model." Is it True or False? 
- [ ] True
  - > Prompt Tuning focuses on optimizing the prompts given to the model using trainable tokens that don’t correspond directly to human language.  The number of tokens you choose to train, however, would be a hyperparameter of your training process.
- [x] False
10.  "PEFT methods can reduce the memory needed for fine-tuning dramatically, sometimes to just 12-20% of the memory needed for full fine-tuning." Is it True or False? 
- [x] True
  - > By training a smaller number parameters, whether through selecting a subset of model layers to train, adding new, small components to the model architecture, or through the inclusion of soft prompts, the amount of memory needed for training is reduced compared to full fine-tuning.
- [ ] False

# Week :three: 

1. Which of the following are true in regards to Constitutional AI? Select all that apply.
   - [x] Red Teaming is the process of eliciting undesirable responses by interacting with a model 
     - > Red Teaming is the process of eliciting undesirable responses, and it is necessary for the first stage of Constitutional AI, as we need to fine-tune the model with those “red team” prompts and revised answers.
   - [x] To obtain revised answers for possible harmful prompts, we need to go through a Critique and Revision process
     - > This process is necessary for Constitutional AI, and its done by asking the model to critique and revise the elicited harmful answers.
   - [x] In Constitutional AI, we train a model to choose between different responses
     - > This is the role of the preference model, that will learn what responses are preferred following the constitutional principles.
   - [ ] For Constitutional AI, it is necessary to provide human feedback to guide the revisions.
2. What does the "Proximal" in Proximal Policy Optimization refer to?
   - [ ] The algorithm's ability to handle proximal policies
   - [x] The constraint that limits the distance between the new and old policy 
     - > The "Proximal" in Proximal Policy Optimization refers to the constraint that limits the distance between the new and old policy, which prevents the agent from taking large steps in the policy space that could lead to catastrophic changes in behavior.
   - [ ] The use of a proximal gradient descent algorithm
   - [ ] The algorithm's proximity to the optimal policy
3. "You can use an algorithm other than Proximal Policy Optimization to update the model weights during RLHF.". Is this true or false? 
    - [x] True
      - > For instance, you can use an algorithm called Q-Learning. PPO is the most popular for RLHF because it balances complexity and performance, but RLHF is an ongoing field of research and this preference may change in the future as new techniques are developed.
    - [ ] False
4. In reinforcement learning, particularly with the Proximal Policy Optimization (PPO) algorithm, what is the role of KL-Divergence? Select all that apply.
   - [x] KL divergence measures the difference between two probability distributions.
     - > KL-Divergence is a mathematical measure of the difference between two probability distributions.
   - [ ] KL divergence encourages large updates to the LLM weights to increase differences from the original model.
   - [ ] KL divergence is used to train the reward model by scoring the differences of the new completions from the original human-labeled ones.
   - [x] KL divergence is used to enforce a constraint that limits the extent of LLM weight updates.
     - > PPO used KL divergence to introduce a constraint that limits the changes to the LLM weights to prevent dramatic changes from the original model.
5. Fill in the blanks: When fine-tuning a large language model with human feedback, the action that the agent (in this case the LLM) carries out is `___` and the action space is the `___`. 
   - [x] Generating the next token, vocabulary of all tokens.
     - > The LLM generates tokens based on the text in the context window, and the probability of all tokens in the vocabulary.
   - [ ] Generating the next token, the context window.
   - [ ] Calculating the probability distribution, the LLM model weights.
   - [ ] Processing the prompt, context window. 
6. How does Retrieval Augmented Generation (RAG) enhance generation-based models?
   - [ ] By increasing the training data size.
   - [x] By making external knowledge available to the model
     - > The retriever component retrieves relevant information from an external corpus or knowledge base, which is then used by the model to generate more informed and contextually relevant responses. This incorporation of external knowledge enhances the quality and relevance of the generated content.
   - [ ] By optimizing the model architecture to generate factual completions.
   - [ ] By applying RL techniques to augment completions.
7. How can incorporating information retrieval techniques improve your LLM application? Select all that apply.
   - [x] Overcome Knowlegde Cut-offs
     - > Retrieving data from external sources enables the model to incorporate information it did not see during training when generating text.
   - [ ] Reduced memory footprint for the model
   - [x] Improve relevance and accuracy of responses
     - > By retrieving from curated, verified datasets you can improve the relevance and accuracy of the model’s completions.
   - [ ] Faster training speed when compared to traditional models
8. What is a correct definition of Program-aided Language (PAL) models?
   - [x] Models that assist programmers in writing code thorugh natural language interfaces.
     - > Program-aided Language (PAL) models are designed to assist programmers in writing code using natural language interfaces. They aim to facilitate the coding process by providing support and guidance through human-like interactions.
   - [ ] Models that enable automatic translation of programming languages to human languages.
   - [x] Models that offload computational tasks to other programs.
     - > It offloads these tasks to a runtime symbolic interpreter such as a python function, which reduces the workload for the LLM and improves accuracy as symbolic interpreters tend to be more precise with computational tasks.
   - [ ] Models that integrate language translation and coding functionalities.
9. Which of the following best describes the primary focus of ReAct?
   - [x] Studying the separate topics of reasoning and acting in LLMs. 
     - > The ReAct framework aims to enhance both language understanding and decision-making capabilities in LLMs by combining reasoning and acting components.
   - [ ] Enhancing language understanding and decision making in LLMs.
   - [ ] Exploring action plan generation in LLMs.
   - [ ] Investigating reasoning abilities in LLMs through chain-of-thought prompting.
10. What is the main purpose of the LangChain framework?
   - [ ] To evaluate the LLM's completions and provide fast prototyping and deployment capabilities. 
   - [ ] To provide prompt templates, agents, and memory components for working with LLMs. 
   - [x] To chaing together different components and create advanced use cases around LLMs, such as chatbots, Generative Question-Answering (GQA), and summarization.
     - > The LangChain framework is built around LLMs and allows the chaining of various components to create more advanced applications for LLMs. It supports use cases like chatbots, Generative Question-Answering (GQA), and summarization.
   - [ ] To connect with external APIs and datasets and offload computational tasks.
