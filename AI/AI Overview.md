---
professor: Anirudhan Adukkathayar C
textbook: "[[AI - A modern approach 3rd Edition.pdf]]"
---

Textbook  
[[AI - A modern approach 3rd Edition.pdf|AI - A Modern Approach]] - by Stuart Russell & Peter Norvig

---

# Unit 1 

2023-09-05
# Chapter 1 : What is AI? 

(imp - write any one definition)
- The branch of CS that is concerned with automation of intelligent behaviour.

![[AI Definition based of different Approaches.png]]

## [[Approaches or Views of AI]] (imp)

- Thinking Humanly
- Thinking Rationally
- Acting Humanly
- Acting Rationally

2023-09-06
## State of Arts

(questions could be asked based on applied AI)

### What can AI do today? What all fields can it include?

- Robotics - self driving cars, vacuum cleaners
- Speech Recognition
- Autonomous planning and scheduling - eg. NASAs autonomous planning agent (there will be latency to send and receive data between mars rover and earth command centre)
- Game playing - eg. IBM's Deep Blue - first computer to beat a world champion in chess
- Spam detection - Classification of messages and calls as spam
- Logistic Planning - eg. DART (Dynamic Analysis and Replanning tool) (planning courier and how to distribute goods)
- Machine Translation - eg. google translate

---

# Chapter 2 : Intelligent Agents

2023-09-11

## What is an agent?

An agent is something that acts. (ps. an agent can be anything - eg. a dog or a robot or kausthubh)

They are expected to
- operate autonomously
- perceive their environment
- persist over prolonged time period
- adapt to change
- create and perceive goals

- Environment / others → constitutes the problem
- Agent → solves the problem

Eg. of a smart vacuum cleaner → the dirt, floor and carpets are the environment & vacuum cleaner is the agent

### Training an agent (reinforcement learning)
- agent will observe the environment
- will perform some action
- will explore different states
- agent will be awarded

![[Reinforcement learning of agent.png]]

## Rational Agents

Rational decisions - decisions based on logical reasoning

- Humans have the ability to make rational decision based based on his/her experience and logical reasoning. (but they don't always make rational decisions). 
- Similarly an agent should be able to make correct decisions based on it's knowledge based on past experience.
	- percept → 
	- percept sequence → 

(imp - percept and percept sequence)

>[!definition]  
>Rational agent : it is agent that does right things and acts rationally so as to achieve the best outcome even when there is uncertainty in knowledge

>[!Mathematical Definition]  
>An agent is a function from percept histories to actions  
>$f : P^* \rightarrow A$
>
>where  
>$P^*$ → percept histories about environment and tasks  
>$A$ → actions
>

## Sensors and actuators

Agent is anything that can be viewed as perceiving its environment through sensors and acting upon the environment through actuators.

- Eg. 1 : Human agent has eyes, ears and other organs for sensors and hands, legs, vocal tract etc. for actuators
- Eg. 2 : Robotic agent → cameras, infrared etc → sensors
- Eg. 3 : Software agent → keystrokes can be sensors


![[Intelligent Agent Wiki.png]]

Percepts → information that are gained from the environment at a particular moment of time with the use of sensors  
Percept sequence → sequence of percepts that are stored in the memory

## Simple Agent Example

Vacuum-cleaner with just two rooms  
![[Vacuum Cleaner Agent Example.png]]

---

2023-09-12

## Good Behaviour: The concept of rationality

**Rationality** = doing the right thing...  
But what does right thing mean? And how do you measure it?

### Rationality at any given depends on 4 things
- Performance measure 
- Agent's prior knowledge of the environment
- Actions that agent can perform
- Agent's percept to date

### Vacuum Cleaner is a rational agent or not? (refer ppt)

It depends!!  

Lets try to measure the rationality #todo
- Performance measure - awards one point for each clean square at each time step
- Prior knowledge → 
- Available actions → left, right and suck
- Agent's percepts to date → 

### Vacuum cleaner is it irrational?

Is it possible to prove that the same agent is irrational?

## Nature of Environment

### 1. Specifying the Task Environment

It is a collection of performance measure, environment, actuators and sensors. (**PEAS**)  
Eg. a self driving tesla

![Task Environment](Task%20Environment.png)
### 2. Properties of Task Environment

- Fully observable vs partially observable task environment
	- fully observable envt. implies that the entire environment is known
- Single agent vs Multi agent
	- eg. an agent playing chess is a 2-agent envt.
- Deterministic vs stochastic
	- deterministic system is if we can predict the next state of the envt. by using the current state
- Episodic vs sequential
	- in sequential envt. the history of the envt will affect the next step
	- in episodic, the next episode does not depend on the actions taken in previous episodes
- Static vs Dynamic
	- #todo
- Discrete vs. continuous
- Known vs. unknown

---
