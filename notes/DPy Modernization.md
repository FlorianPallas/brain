## Dependencies
DecentralizePy has been updated to the newest Python version, along with all dependencies. It has also been migrated to use the UV package manager, which is a modern alternative to previous virtual environment managers like conda.

## Code Quality
In the last year type inference and explicit typing support was greatly improved. This allows for safer code. With the help of coding agents, the code has been modernized to be easier for type inference. Bad patterns that masked real typed have been replaced with easier to infer alternatives, without breaking existing behavior. 

## GPU Support
Previously the implementation of DecentralizePy was lacking code to move data to a GPU if configured. This has been added. With the feature switches the user can choose between three backends: CPU, CUDA (NVIDIA), ROCM (AMD).

## Runner
To facilitate deployments over multiple machines, runner scripts were added, giving users the ability to configure remote hosts. Configurations can then be dispatched to remotes with a single command. Results will be aggregated locally for review.

## Communication
Previously nodes communicated their model weights, which can be heavy and is not very realistic compared to real systems. Usually deltas are exchanged. DecentralizePy has been extended to support delta communication.

## Agentic Coding
Using coding agents has become a central part of modern programming. To make it easier for agents to understand and work with the project, documentation has been added.
