#	Language Models for Dynamic Hint-Giving in Video Games
LLM  •  SLM  •  Game Engineering  •  HCI  •  AI

Providing helpful hints in logic-heavy games is difficult. Standard hint systems are usually static — either offering vague advice or spoiling the solution entirely. Dynamic implementations require significant effort to analyze and handle all possible failure states.  This project explores the use of Language Models (LLMs and SLMs) to provide dynamic, context-aware assistance. Using an existing indie game about electrical installations as a testbed (source code provided), the goal is to develop a system that reads the player's current wiring solution, encodes the puzzle rules and current state, and provides natural-language guidance through a Language Model — without giving away the solution.

## Research Questions
*	RQ1 (Representation): How can a non-linear wiring graph and specific level requirements be serialized into a text-based format that allows a language model to identify both electrical faults and missing functional goals?
*	RQ2 (Instruction Tuning): How do different prompting strategies affect the player's ability to solve an installation puzzle without further help?
*	RQ3 (Performance Trade-offs): How do Small Language Models compare to Large Language Models in reasoning about causal relationships between electrical flow and abstract puzzle objectives?

## Tasks
*	State Serialization: Map the game's internal state into a structured text format (e.g., YAML, JSON, natural language), including wiring logic, requirements, current solution, and potential short-circuits.
*	AI Integration: Build a pipeline to send the encoded state to a language model and retrieve a structured hint.
*	Hint Strategy Design: Develop a prompt framework that prevents spoilers and instead guides the player toward identifying their own mistakes.
*	Implementation and Evaluation: Integrate the system into the game UI and document the model's success rate in identifying common errors through a user study.
