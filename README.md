# Foundation: Introduction to LangGraph
Link: [https://academy.langchain.com/courses/intro-to-langgraph/](https://academy.langchain.com/courses/intro-to-langgraph/)

## Module 1

### Lesson 1
Understood how langgraph helps improve agents using langsmith studio. Also understood the difference between router and fully autonomous agents.

Tweaks and learnings:
- Edited the studio files ([agent.py](module1/studio/agent.py), [router.py](module1/studio/router.py)) to ensure they work with Anthropic

### Lesson 2
Link: [Lesson2.ipynb](module1/lesson2.ipynb)\
Learnt how to create and execute nodes and edges for agentic AI

Tweaks and learnings:
- Added `node_4` alongside the other moods
- Learnt how to invoke graphs and how graphs work

### Lesson 3
Link: [simple.py](module1/studio/simple.py)
Explored the langgraph studio UI and learnt how to inspect graph invocations step-by-step.

Tweaks:
- Added `node_4` from [lesson2](module1/lesson2.ipynb) in [Simple Agent example](module1/studio/simple.py)

### Lesson 4
Link: [lesson4.ipynb](module1/lesson4.ipynb)

Tweaks and learnings:
- Learnt about reducers
- Solved the classic LLM problem of counting the occurrence of letter in given text with agentic AI (overkill though)

### Lesson 5
Link: [lesson5.ipynb](module1/lesson5.ipynb)

Tweaks and learnings:
- Used router to use multiple tools
- Understood how to route between text and different tools
- Changed the code to include another model and try out routing
- Also interactively visualized the model output using langgraph studio