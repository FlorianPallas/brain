## Facts
- Mi. 22.04.2026 - 12:00
- 20 Minute presentation
- 10 Minute discussion
- Participants: DSN staff, head professor, and some students
- Content
	- Should include a hook
	- Presentation must go into depth on technical terms, no prior knowledge of ML should be required to follow the presentation
	- Clear statement of the research questions is required
	- Clear statement of tasks and an associated timeline is required

## TODO
- [ ] Hook
- [ ] x

## Questions
- Should I introduce myself in detail?

## Reminders
- DFL is not inherently private - Needs concepts like Differential Privacy

## Journey
A rough overview of themes and the transitions between them, so the presentation

- The Hook
	- Global AI race of few companies
	- Privacy concerns
- The Utopia
	- DFL is great for a lot of use cases
	- No severs, No dependence, Private
- The Reality
	- Large attack surface for privacy, robustness, and efficiency
	- -> Mitigations exist, lets build the perfect system
- PRE Trilemma
	- A perfect system does not exist
	- Is this all a waste of time? - No
	- -> We need to make trade-offs, like always in computer science
- Research Question
	- How can we assess the impact of trade-offs?
	- How viable are DFL systems in reality?
- Methodology
	- We build a DFL system with common mitigations
	- We look at different realistic scenarios
	- We build a framework for these assessments
- The Plan
	- Tasks
	- Timeline
	- Hopes

## Slides
Actual bullet points of the final presentation. One heading represent a single slide. Expected duration of the slide is stated.

### Introduction
^2min
- Personal introduction
- Hook:
	- AI Race of few companies, hard to compete
	- Independence from foreign states more important than ever
	- Growing Privacy concerns and push towards data sovereignty
	- EU push towards Open Source, Community-driven works
- Examples
	- Hospitals
	- Keyboard Predictions
	- Car Fleets

### Machine Learning Methods
^1min
- What is CL?
	- Here: Image Classifier, CIFAR-10
- What is FL?
	- Training on device, central aggregation
- What is DFL?
	- Network of nodes, aggregation and training on device

### Characterizing ML systems
^1min
- Privacy
	- Can training data be deduced from outputs or weights?
- Robustness
	- How resistant is the model against attacks?
- Efficiency
	- How accurate is the model in comparison with the training costs

### Improving Privacy
^2min
- Attacks
	- Membership inference, leakage, prompt engineering
	- e.g. Gradient Leakage
	- https://arxiv.org/abs/1906.08935
- Mitigations
	- Differential privacy
	- Adds noise before exchanging gradients

### Improving Robustness
^2min
- Attacks
	- Model poisoning, data poisoning, DoS, etc.
	- e.g. Poisoning Image Generators so they produce garbage
	- https://mag.uchicago.edu/uchi-con
- Mitigations
	- Trimmed mean aggregation
	- Remove statistical outliers from updates

### Improving Efficiency
^1min
- Challenges
	- Bandwidth, compute, or latency limits
- Mitigations
	- Compression, more local training rounds, network topology improvements

 ### PRE Trilemma
^2min
- In worst-case scenario
- Three properties, pick two
- We need to make trade-offs
- Existing real-world applications already do this

### Thesis Proposal
^1min
- How relevant is the PRE trilemma for real-world applications?
- How can we make informed decisions about our implementations?

### Simulating DFL systems
^1min
- Simulation
- DecentralizePy

### Modeling real-world scenarios
^1min
- Certain attack vectors more likely
- Trade-offs are result of these circumstances
- -> Implement common mitigations
- -> Adjust parameters

### Evaluating scenarios
^1min
- Privacy
	- Differential Privacy with $\epsilon$ budget
	- Membership Inference Attack
- Robustness
	- Model Poisoning with $\eta$ fraction of malicious nodes
	- Success rate of a Model Poisoning Attack
	- How many previously correct predictions are now incorrect?
- Efficiency
	- Compression until bandwidth limit $\delta$ is reached
	- Compare accuracy, time, bandwidth to baseline without attacks

### Tasks
^2min
- A lot of research has already been conducted
- DecentralizePy is already running on DSN hardware
- Training
	- Implement differential privacy
	- Implement trimmed mean aggregation
	- Reuse existing compression
- Attacks
	- Implement model poisoning nodes
	- Use existing tools to perform membership inference attacks
- Tooling
	- Modernize code
	- Build tooling for attacks and evaluation
- Stretch goals
	- Play with network sizes
	- Test new scenarios
	- Test new datasets

### Writing
^1min
- Abstract
- Background
- Implementation details
- Scenario definitions
- Discussion of results
- Reflection on DecentralizePy
- Further research

## Timeline
^1min


## Outro
^1min
- References
- Questions
