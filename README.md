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

### Lesson 6
Link: [lesson6.ipynb](module1/lesson6.ipynb)

Tweaks and learnings:
- Learnt about ReAct
- Learnt how to iteratively access tools until we obtain final results
- Added another tool and ran a prompt that accesses all the tools at least once serially
- Used langchain to check the trace of tool runs and LLMs

### Lesson 7
Link: [lesson7.ipynb](module1/lesson7.ipynb)

Tweaks and learnings:
- Learnt how to use `persistence`/ `MemorySaver` to retain previous states as context for the follow up questions
- Implemented another custom tool call `ascii_to_letter` and made it work with the pipeline

## Module 2

### Lesson 1
Link: [lesson1.ipynb](module2/lesson1.ipynb)

Tweaks and learnings:
- Learnt how to validate type hints using PydanticState to enure the return type remains consistent
- Learnt about dataclasses
- Implemented an extra code to validate that PydanticState is working as expected

### Lesson 2
Link: [lesson2.ipynb](module2/lesson2.ipynb)

Tweaks and learnings:
- Learnt how to update values in state after branching to not break the model
- Read the documentation to understand how it works
- Learnt about custom reducer to implement own logic
- Played around with simple examples to understand the lesson

### Lesson 3
Link: [lesson3.ipynb](module2/lesson3.ipynb)

Tweaks and learnings:
- Learnt how to make multiple schema including private schema, input schema and output schema
- Tweaked the code to change output schema of the models

### Lesson 4
Link: [lesson4.ipynb](module2/lesson4.ipynb)

Tweaks and learnings:
- Explored advanced message handling techniques in LangGraph using `MessagesState` for managing conversations
- Learned the difference between filtering (selecting specific messages) and trimming (token-based message truncation)
- Modified all code to work with Claude (Anthropic) instead of OpenAI - updated to use `ChatAnthropic` with claude-haiku-4-5 model
- Added comparison example demonstrating practical differences between filtering and trimming approaches
- Learned how to manage long-running conversations efficiently to reduce token usage and latency

### Lesson 5
Link: [lesson5.ipynb](module2/lesson5.ipynb)

Tweaks and learnings:
- Learned how to create custom state schemas by extending `MessagesState` with additional keys like `summary`
- Learned about threads - how they work like Slack channels to maintain separate conversation contexts
- Added thread isolation demo showing how different thread IDs maintain completely separate conversations simultaneously
- Understood how checkpointers save state after each step, enabling interruption and resumption of conversations

### Lesson 6
Link: [lesson6.ipynb](module2/lesson6.ipynb)

Tweaks and learnings:
- Learned how to use external database checkpointers for persistent memory beyond in memory storage
- Understood the difference between in-memory and file-based SQLite database
- Renamed the state field
- Updated all prompts and helper functions


## Module 3

### Lesson 1
Link: [lesson1.ipynb](module3/lesson1.ipynb)

Tweaks and learnings:
- Explored two main streaming modes
- Created helper function to extract and display specific event metadata
- Learned how to use langgraph sdk client to stream from deployed graphs

### Lesson 2
Link: [lesson2.ipynb](module3/lesson2.ipynb)

Tweaks and learnings:
- Learned about breakpoints
- Implemented user approval workflow to control tool execution before running
- Configured all code to use Claude haiku 4.5
- Explored breakpoints with LangGraph API

### Lesson 3
Link: [lesson3.ipynb](module3/lesson3.ipynb)

- Learnt how to use breakpoints to enable interruptions from user to update state
- Added division feature too with the same feature set as multiplication

### Lesson 4
Link: [lesson4.ipynb](module3/lesson4.ipynb)

Tweaks and learnings:
- Learnt about dynamic breakpoints for runtime based conditional interruptions
- Learnt about self interrupting graphs based on conditions evaluated within nodes

### Lesson 5
Link: [lesson5.ipynb](module3/lesson5.ipynb)

Tweaks and learnings:
- Learnt to use time travel for debugging
- Learnt about `get_state_history` to see past execution states
- Learnt about forking
- Added similar functionalities for modulo function

## Module 4

### Lesson 1
Link: [lesson1.ipynb](module4/lesson1.ipynb)

Tweaks and learnings:
- Learnt about executing multiple nodes at the same time and merge them
- Learnt about reducers and custom reducers
- Implemented code for Claude haiku 4.5