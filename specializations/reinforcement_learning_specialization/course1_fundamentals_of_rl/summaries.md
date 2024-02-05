
# 1. Course 1️⃣ - Fundamentals of Reinforcement Learning

- [1. Course 1️⃣ - Fundamentals of Reinforcement Learning](#1-course-1️⃣---fundamentals-of-reinforcement-learning)
  - [2. Week 🕐](#2-week-)
    - [2.1. The K-Armed Bandit Problem](#21-the-k-armed-bandit-problem)
      - [2.1.1. Sequential Decision Making with Evaluative Feedback](#211-sequential-decision-making-with-evaluative-feedback)
    - [2.2. What to Learn? Estimating Action Values](#22-what-to-learn-estimating-action-values)
      - [2.2.1. Learning Action Values](#221-learning-action-values)
      - [2.2.2. Estimating Action Values Incrementally](#222-estimating-action-values-incrementally)
    - [2.3. Exploration vs Exploitation Tradeoff](#23-exploration-vs-exploitation-tradeoff)
      - [2.3.1. What is the trade-off?](#231-what-is-the-trade-off)
      - [2.3.2. Optimistic Initial Values](#232-optimistic-initial-values)
      - [2.3.3. Upper-Confidence Bound (UCB) Action Selection](#233-upper-confidence-bound-ucb-action-selection)
  - [3. Week 🕑](#3-week-)
  - [4. Week 🕒](#4-week-)
- [5. Week 🕓](#5-week-)


On this page we will write down the learnings from the materical of course 1️⃣. This will contain the summaries of each video of the specialization. Note that these summaries are completely the content of the [University of Alberta](https://www.ualberta.ca/index.html) and [Coursera](https://www.coursera.org/). Thus, all the credit goes to them. This page should simply hold as a reference point for interested learners to quickly come back to the learned content.

## 2. Week 🕐

### 2.1. The K-Armed Bandit Problem
#### 2.1.1. Sequential Decision Making with Evaluative Feedback

- __Decision making under uncertainty__ can be formalized by the __k-armed bandit problem__
- Fundamental ideas: __actions__, __rewards__, __value functions__

### 2.2. What to Learn? Estimating Action Values
#### 2.2.1. Learning Action Values

- __Sample-average method__ can be used to estimate action values
- The __greedy action__ is the action with the highest value estimate

<u>Action-Values</u>

$$
\begin{align*}
q_*(a) &\dot{=} \mathbb{E}[ R_t | A_t = a ] \qquad \forall a \in \{1, \dots, k\} \\
       &= \sum_r \underbrace{p(r | a)}_{\text{prob. of observing reward} \; r}r
\end{align*}
$$ 

- The __value__ of an action $a$ is the __expected reward__ when that action is taken

<u>Sample-Average Method</u>

$$
\begin{align*}
    Q_t(a) \dot{=} \frac{\text{sum of rewards when} \; a \; \text{taken prior to} \; t}{\text{number of times} \; a \; \text{taken prior to} \; t} = \frac{\sum_{i=1}^{t-1}R_i}{t-1} = \frac{1}{t-1} \sum_{i=1}^{t-1}R_i
\end{align*}
$$

- Can be used to estimate action values $Q(a)$

#### 2.2.2. Estimating Action Values Incrementally

- Derived incremental sample average method
- Generalized the __incremental update rule__ into a more __general update rule__
- A __constant stepsize parameter__ can be sued to solve __a non-stationary bandit problem__

<u>Incremental Update Rule</u>

$$
\begin{align*}           
    \underbrace{Q_{t+1}}_{NewEstimate} 
            &= \underbrace{Q_t}_{OldEstimate} +
               \underbrace{\alpha_t}_{StepSize}(
               \underbrace{R_t}_{Target} -
               \underbrace{Q_t}_{OldEstimate})
\end{align*}
$$

### 2.3. Exploration vs Exploitation Tradeoff
#### 2.3.1. What is the trade-off?

- We discussed the __tradeoff__ between __exploration and exploitation__
- We introduced __epsilon-greedy__ which is a simple method for balancing exploration and exploitation

<u>Exploration versus Exploitation</u>

- __Exploration__ - _improve_ knowledge for _long-term_ benefit
- __Exploitation__ - _exploit_ knowledge for _short-term_ benefit

<u>Epsilon-Greedy Action Selection</u> 

$$
\begin{align*}
    A_t \leftarrow \left \{
    \begin{array}{ll}
        \text{argmax}_a Q_t(a) & \text{with probability} \; 1 - \epsilon \\
        a \sim Uniform(\{a_1, \dots, a_k \}) & \text{with probability} \; \epsilon 
    \end{array}
\right.
\end{align*}
$$

- is a method to choose when to exploit and when to explore

#### 2.3.2. Optimistic Initial Values

- __Optimistic initial values__ encourage _early exploration_ 
- Described limitations of __optimistic initial values__

<u>Limitations of optimistic initial values</u>

- Optimistic initial values only _drive early exploration_
- They are not well-suited for _non-stationary problems_ 
- We may not know what the _optimistic initial value_ should be

#### 2.3.3. Upper-Confidence Bound (UCB) Action Selection

- __Upper-Confidence Bound action-selection__ uses _uncertainty_ in the value estimates for balancing exploration and exploitation

<u>Upper-Confidence Bound (UCB) Action Selection</u>

$$
\begin{align*}
    A_t \dot{=} argmax \Big[ \underbrace{Q_t(a)}_{\text{Exploit}} + c \underbrace{\sqrt{\frac{ln \, t}{N_t(a)}}}_{\text{\text{Explore}}} \Big]
\end{align*}
$$

## 3. Week 🕑

## 4. Week 🕒

# 5. Week 🕓