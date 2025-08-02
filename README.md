# discovery_DCR_from_Text


## Experimental Setup


## Prompting Strategy Overview

Role = Entity assigned to one or more Activities
Event = Activities that are executed or performed, and Events that happen
Rule = Deontic/Defeasible Constraint between Events (We use: Condition, Response, Exclude, Include, Milestone, as defined by DCR)

### Pipelines

Pipeline A - Instruct LLM to find Roles, then Activities, and then Rules based on previous findings. The Rules are to be found all at ones.
Pipeline B - Instruct LLM to find Roles, then Activities, and then Rules based on previous findings. Rules of one type are found independently of the other types. Previous found constraints are disregarded.

### Prompts

Prompt_1 - only uses simple context
Prompt_2 - add in-context learning
Prompt_3 - add one correct example (one shot)
Prompt_4 - add another correct example and one wrong example (three shot)
Prompt_5 - add annotation guidelines to in-context learning

