## Recap 

First we call the system prompt..

![image](https://github.com/user-attachments/assets/2fd08b00-af8e-4bdf-9b9d-9cd790f58512)

we have Thought and Action

we still have 2 tools which is the function that they can do.

After that we return the observation to loop back to the prompt.

Learn more about the ReAct paper here : https://arxiv.org/abs/2210.03629

Next, we will replace the formatted variable so we can have prompt templates.

## LangChain: Prompts use for prompt templates

![image](https://github.com/user-attachments/assets/84946f81-6ded-49f1-a961-4ed86cbb3557)

## LangChain: Tools (Function that LLM can do)

![image](https://github.com/user-attachments/assets/b0dc3cb6-063d-411d-9aad-1fcec2480ea6)

New in LangGraph :

Most code will be loop Langraph we have this 3 new features.

* Cyclig Graphs - control flows
* Persistence bulit-in - Multiple agents and conversations remembering iterations and actions
* Human-in-the-loop

![image](https://github.com/user-attachments/assets/e6460575-bbe4-40ef-8503-0cbf35c195d1)

aimed at agent and multi-agent flows.

Node : LLM or functions
Edges : connected
Conditional edges: decisions

* Agent state it's mean you can resume at any state

![image](https://github.com/user-attachments/assets/a1db502f-931c-4a7c-8633-8ad661224d8a)

For the simple agentstate it's operator add which is not overrides the extisting values.

Complex state : agent action and agent observation throughout the graph.

![image](https://github.com/user-attachments/assets/2858cfa4-5ef5-428f-afb8-716163b098fd)

from langchain_core.messages import AnyMessage, SystemMessage, HumanMessage, ToolMessage This is the standard messages











