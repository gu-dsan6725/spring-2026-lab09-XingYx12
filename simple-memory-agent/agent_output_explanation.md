
# 1.Session Information 

* user_id = demo_user indicates person that uses the system
* agent_id = memory-agent indicates agent that been used in the session
* session = e0422374 indicates a single run of the system

# 2.Memory Types 

* Factual memory: user's name is 'Alice' and 'software engineer specializing in Python' in turn 1
* Semantic memory: Knoweldge about NN in turn 6
* Preference memory: user prefer clean, maintainable code and favorite programming language is Python in turn 4
* Episodic memory:I'm working on a machine learning project using scikit-learn. in turn 2


# 3. Tool Usage Patterns
insert_memory: in turn 1, 2, 4. The user provided the information about her self and ask the agent to remember
automatic: When user did not provide any information taht need to be stored. The agent will retrive information from storage to answer questions and keep the conversion going. 


# 4.Memory Recall - Which turns trigger memory search? How do you know?
Turn 3, 5, 7 trigger memory search. Since these questions were stroed in previous insrt_memory. And if the information can not be answered by using system, the agent will try to call memory recall to find answer.

# 5.Single Session - Explain how all 7 turns happen in ONE session and why that matters

To ensure all the important information from early convrsation can be stored by agent. Since the system will not store any information to the disk. If we do not run all 7 turns in one session. All the savd preference from user will lost.

