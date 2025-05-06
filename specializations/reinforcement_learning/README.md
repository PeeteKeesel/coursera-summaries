# Reinforcement Learning Specialization

This folder contains notebooks as well as personal summaries and notes for the [Reinforcement Learning Specializations](https://www.coursera.org/specializations/reinforcement-learning) from the [University of Alberta](https://www.ualberta.ca/index.html) on [Coursera](https://www.coursera.org/). The notebooks are contents of the course. The solutions are my own work. All the rest has been created by Coursera and the University of Alberta and thus, the credit goes to

```
Coursera
University of Alberta
```

## 🎯 Learning Objectives 

- Course 1️⃣ 

<details>
  <summary>show learning objectives</summary>

```
Week 🕐 
  - Understand the prerequisites, goals and roadmap for the course.
Week 🕑
  - Understand Markov Decision Processes (MDP)
  - Describe how the dynamics of an MDP are defined
  - Understand the graphical representation of a Markov Decision Process
  - Explain how many diverse processes can be written in terms of the MDP framework
  - Describe how rewards relate to the goal of an agent
  - Understand episodes and identify episodic tasks
  - Formulate returns for continuing tasks using discounting
  - Describe how returns at successive time steps are related to each other
  - Understand when to formalize a task as episodic or continuing
Week 🕒
	- Recognize that a policy is a distribution over actions for each possible state
	- Describe the similarities and differences between stochastic and deterministic policies
	- Generate examples of valid policies for a given MDP
	- Describe the roles of state-value and action-value functions in reinforcement learning
	- Describe the relationship between value functions and policies
	- Create examples of valid value functions for a given MDP
	- Derive the Bellman equation for state-value functions
	- Derive the Bellman equation for action-value functions
	- Understand how Bellman equations relate current and future values
	- Use the Bellman equations to compute value functions
	- Define an optimal policy
	- Understand how a policy can be at least as good as every other policy in every state
	- Identify an optimal policy for given MDPs
	- Derive the Bellman optimality equation for state-value functions
	- Derive the Bellman optimality equation for action-value functions
	- Understand how the Bellman optimality equations relate to the previously introduced Bellman equations
	- Understand the connection between the optimal value function and optimal policies
	- Verify the optimal value function for given MDPs
Week 🕓
	- Understand the distinction between policy evaluation and control
	- Explain the setting in which dynamic programming can be applied, as well as its limitations
	- Outline the iterative policy evaluation algorithm for estimating state values under a given policy
	- Apply iterative policy evaluation to compute value functions
	- Understand the policy improvement theorem
	- Use a value function for a policy to produce a better policy for a given MDP
	- Outline the policy iteration algorithm for finding the optimal policy
	- Understand “the dance of policy and value”
	- Apply policy iteration to compute optimal policies and optimal value functions
	- Understand the framework of generalized policy iteration
	- Outline value iteration, an important example of generalized policy iteration
	- Understand the distinction between synchronous and asynchronous dynamic programming methods
	- Describe brute force search as an alternative method for searching for an optimal policy
	- Describe Monte Carlo as an alternative method for learning a value function
	- Understand the advantage of Dynamic programming and “bootstrapping” over these alternative strategies for finding the optimal policy
```

</details>

- Course 2️⃣ 

<details>
  <summary>show learning objectives</summary>

```
Week 🕐 : Monte-Carlo Methods for Prediction and Control
  - Understand the prerequisites, goals and roadmap for the course.
Week 🕑
Week 🕒
Week 🕓
```

</details>


- Course 3️⃣

## 🏛️ Structure

The specialisation is structured into three courses. Each course covers a multitude of topics split into three to four weeks. Most weeks terminate with a combination of quizzes and labs (some only contain one of the two). The "📖Notes" column contains a notebook with summaries and notes for each course.

<table>
  <tr>
    <th>Module</th>
    <td>💡Topic</td>
    <th>🔬Lab</th>
    <th>📝Quizzes</th>
    <th>📖Notes</th>
  </tr>
  <!-- ------------------------------------------------------------ -->
  <!-- COURSE 1 -->                
  <!-- ------------------------------------------------------------ -->
  <tr>
    <td colspan="5" align="center">
      Course 1️⃣:<br><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course1_fundamentals_of_rl">
        <code>Fundamentals of Reinforcement Learning</code>
      </a>     
    </td>
  </tr>
  <tr>
    <td rowspan="1" align="center">1️⃣</td>
    <td>An Introduction to Sequential Decision-Making</td>
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course1_fundamentals_of_rl/C1W1_Assignment.ipynb">ipynb</a></td>
    <td rowspan="1">
        <a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course1_fundamentals_of_rl/quiz_w1.md">quizzes</a>
    </td>
    <td rowspan="4">
        <a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course1_fundamentals_of_rl/summaries_C1.ipynb">ipynb</a>    
    </td>
  </tr>
  <tr>
    <td rowspan="1" align="center">2️⃣</td>
    <td>Markov Decision Processes</td>
    <td>None</td>
    <td rowspan="1">
        <a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course1_fundamentals_of_rl/quiz_w2.md">quizzes</a>
    </td>
  </tr> 
  <tr>
    <td rowspan="1" align="center">3️⃣</td>
    <td>Value Functions & Bellman Equations</td>
    <td>None</td>
    <td rowspan="1">
        <a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course1_fundamentals_of_rl/quiz_w3.md">quizzes</a>
    </td>
  </tr> 
  <tr>
    <td rowspan="1" align="center">4️⃣</td>
    <td>Dynamic Programming</td>
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course1_fundamentals_of_rl/C1W4_Assignment.ipynb">ipynb</a></td>
    <td rowspan="1">
        <a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course1_fundamentals_of_rl/quiz_w4.md">quizzes</a>
    </td>
  </tr> 
  <!-- ------------------------------------------------------------ -->
  <!-- COURSE 2 : Sample-Based Learning Methods -->                
  <!-- ------------------------------------------------------------ -->
  <tr>
    <td colspan="5" align="center">
      Course 2️⃣:<br><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course2_sampled_based_learning_methods">
        <code>Sample-Based Learning Methods</code>
      </a>     
    </td>
  </tr>   
  <tr>
    <td rowspan="1" align="center">2️⃣</td>
    <td>Monte-Carlo Methods for Predition & Control</td>
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course2_sample_based_learning_methods/C2M2_Assignment_Blackjack.ipynb">ipynb</a></td>
    <td rowspan="1">
        <a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course2_sample_based_learning_methods/quiz_m2.md">quizzes</a>
    </td>
    <td rowspan="1">
        <a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course2_sample_based_learning_methods/summaries_C2M2.ipynb">ipynb</a>    
    </td>   
  </tr>
  <tr>
    <td rowspan="1" align="center">3️⃣</td>
    <td>Temporal Difference Learning Methods for Prediction</td>
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course2_sample_based_learning_methods/C2M3_Assignment_TD0.ipynb">ipynb</a></td>
    <td rowspan="1">
        <a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course2_sample_based_learning_methods/quiz_m3.md">quizzes</a>
    </td>
    <td rowspan="1">
        <a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course2_sample_based_learning_methods/summaries_C2M3.ipynb">ipynb</a>    
    </td>     
  </tr> 
  <tr>
    <td rowspan="1" align="center">4️⃣</td>
    <td>Temporal Difference Learning Methods for Control</td>
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course2_sample_based_learning_methods/C2M4_TODO.ipynb">ipynb</a></td>
    <td rowspan="1">
        <a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course2_sample_based_learning_methods/quiz_m4.md">quizzes</a>
    </td>
    <td rowspan="1">
        <a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course2_sample_based_learning_methods/summaries_C2M4.ipynb">ipynb</a>    
    </td>     
  </tr> 
  <tr>
    <td rowspan="1" align="center">5️⃣</td>
    <td>Planning, Learning & Acting</td>
    <td><a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course2_sample_based_learning_methods/C2M5_Assignment.ipynb">ipynb</a></td>
    <td rowspan="1">
        <a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course2_sample_based_learning_methods/quiz_m5.md">quizzes</a>
    </td>
    <td rowspan="1">
        <a href="https://github.com/PeeteKeesel/coursera-summaries/blob/main/specializations/reinforcement_learning/course2_sample_based_learning_methods/summaries_C2M5.ipynb">ipynb</a>    
    </td>     
  </tr>       
</table>

## 📚 Resources
