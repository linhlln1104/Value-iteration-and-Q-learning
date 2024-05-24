## Reinforcement Learning Project

### Introduction

This project focuses on implementing value iteration and Q-learning algorithms. The agents will be tested on various environments, including Gridworld, Crawler, and Pacman. This project working on `python 3.7`

### Files

#### Files to Edit:
- `valueIterationAgents.py`: Implement a value iteration agent for solving known MDPs.
- `qlearningAgents.py`: Implement Q-learning agents for Gridworld, Crawler, and Pacman.
- `analysis.py`: Answer questions and provide analysis for the project.

#### Files to Read but NOT Edit:
- `mdp.py`: Defines methods on general MDPs.
- `learningAgents.py`: Defines base classes for ValueEstimationAgent and QLearningAgent.
- `util.py`: Utilities, including `util.Counter` useful for Q-learners.
- `gridworld.py`: Gridworld implementation.
- `featureExtractors.py`: Classes for extracting features on (state, action) pairs used for the approximate Q-learning agent.

#### Files to Ignore:
- `environment.py`
- `graphicsGridworldDisplay.py`
- `graphicsUtils.py`
- `textGridworldDisplay.py`
- `crawler.py`
- `graphicsCrawlerDisplay.py`
- `autograder.py`
- `testParser.py`
- `testClasses.py`
- `test_cases/`
- `reinforcementTestClasses.py`

### Running the Autograder

You can run the autograder for all questions using the following command:

```bash
python autograder.py
```

### To run the autograder for a specific question, use:

```bash
python autograder.py -q <question_number>
```

### For example, to test question 2:
```bash
python autograder.py -q q2
```

### To run a specific test case, use:
```bash
python autograder.py -t <test_case_path>
```

### Running Gridworld
#### You can run Gridworld in manual control mode using the arrow keys:
```bash
python gridworld.py -m
```

#### To run Gridworld with a specific layout, use:
```bash
python gridworld.py -g <layout_name>
```

#### For example:
```bash
python gridworld.py -g MazeGrid
```

### Running Pacman
#### To run Pacman with a Q-learning agent:
```bash
python pacman.py -p PacmanQAgent -x 2000 -n 2010 -l smallGrid
```
#### You can also specify different layouts and learning parameters using additional flags.

### Testing the Approximate Q-Learning Agent
#### To test the approximate Q-learning agent with custom feature extractor:
```bash
python pacman.py -p ApproximateQAgent -a extractor=SimpleExtractor -x 50 -n 60 -l mediumGrid 
```

### Grading
#### To grade your implementation, use the autograder with the appropriate question number:
```bash
python autograder.py -q <question_number>
```

