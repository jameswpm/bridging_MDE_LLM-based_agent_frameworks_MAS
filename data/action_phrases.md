### For each term captured from the selected frameworks, **at least** 2 action phrases were elaborated to capture their relations and potential attributes. Plural form were used to represent some level of cardinality. Nouns indicates entities or attributes, while verbs indicate actions.

#### Agent
- Agents use Tools to perform Tasks.
- Agents have Memory components to store Context and history.
- Agents rely on Models to interpret input and generate responses.
- Agents follow given Instructions.
- Agents have access to external Knowledge.
- Agents can perform Reasoning to solve problems.
- Agents use Storage to persist their State.
- Agents execute code at runtime via an Interpreter.
- Agents have unique identifiers (addresses, names, or IDs).
- Agents may be public-facing or private (depending on deployment).
- Agents can be classified by type or specialization.
- Agents may have a Goal to achieve.
- Agents have a current State at any given time.
- Agents can form or join Teams of agents.
- Agents can act based on their reasoning processes or according to a Workflow.
- Agents might use retrieval mechanisms (like RAG) to fetch relevant knowledge when needed.

#### Tool
- Tools interface with external systems or APIs (the Environment).
- Tools perform one or more Tasks for agents.
- Hooks may intercept or modify a Tool's execution when triggered.

#### Memory
- Memory stores information about Agents, Sessions, and User interactions (e.g., context, history, summaries).
- Memory can be short-term (ephemeral, per Session) or long-term (persistent across sessions).
- Memory implementations vary, but a common approach uses a VectorDB to store semantic embeddings.

#### Model
- Models interpret Prompts to understand user or agent requests.
- Models generate responses or actions based on input and their training.
- Models support reasoning capabilities through pretraining or fine-tuning.

#### Knowledge
- Knowledge consists of external or domain-specific information accessible by Agents.
- Knowledge often resides outside an agent's internal state (e.g., in documents, databases, or knowledge bases).
- Knowledge can be loaded into Memory for temporary use or stored in Storage for long-term use.

#### Reason
- Reasoning is performed by Agents to analyze information and make decisions.
- Reasoning uses the agent's Knowledge and Memory to infer actions.
- Reasoning processes can involve multiple logical steps or planning.

#### Storage
- Storage persistently saves Agent States and data across sessions.
- Storage resources may be shared by Agents in the same Team.
- Storage can hold large or long-term data (logs, knowledge bases, files, etc.).

#### Prompt
- Prompts guide agents by specifying Tasks, Instructions, or context.
- Prompts can be provided by Users or generated automatically.
- Prompts may be mutable and updated during interactions.
- Prompts can be validated against an Input Schema.
- Prompts may be based on a Prompt Template.

#### Team
- Teams use coordination strategies to organize agent collaboration.
- Team members may share Memory, Storage, and Knowledge resources.
- Teams may assign roles or designate leader agents.

#### State
- An Agent's State includes its current data or context at a given time.
- States can be shared between Agents in the same Team for coordination.
- State information may be persisted to Storage or cached in Memory.

#### Task
- Tasks are specific objectives or jobs for Agents (or agent Teams) to perform.
- Tasks may be defined by Users or by other agents.
- Agents or Teams may succeed or fail in completing Tasks.

#### Environment
- The Environment includes external systems, data sources, and Users outside the Agents.
- Tools allow agents to interact with or manipulate the Environment.
- Agents can transform observed environmental information into internal Knowledge.

#### VectorDB
- VectorDB is a specialized database for storing high-dimensional embeddings.
- VectorDBs are commonly used to implement semantic Memory for Agents.
- VectorDB stores information in vector form (via embeddings) for similarity-based retrieval.

#### Hook
- A hook is a function triggered by specific events or conditions during agent execution.
- Hooks can intercept, extend, or modify tool or agent behavior when activated.

#### User
- A User is an external actor (person or team) who interacts with agents.
- Users can provide Prompts or input to guide the Agent.
- Users may interact with agents through various interfaces (e.g., chat, UI, command-line).

#### RAG
- RAG (Retrieval-Augmented Generation) is a technique where relevant information is retrieved from an external source to augment an agent's prompt.
- RAG often uses a VectorDB of embeddings to fetch context for the model.
- RAG enhances language generation with up-to-date or domain-specific Knowledge.

#### Workflow
- A workflow is a deterministic sequence of steps with Transitions defining the execution flow.
- Workflows consist of defined Steps and Transitions between them.
- Workflows can be pre-defined at development time or constructed/modified by Users at runtime.

#### Input Schema
- An input schema defines the structure and validation rules for an agent's input.
- Input schemas can be formally specified using structured languages (e.g., JSON Schema).

#### Goal
- A goal is the desired outcome or state that an agent aims to achieve.
- Agents work towards achieving their goals.
- Goals can be defined by users and may be represented in the agent's state.

#### Session
- A Session is a collection of interactions linking a user and an agent over time.
- Session information may be stored in Memory or persisted in Storage.

#### Direct LLM Call
- A Direct LLM call is a single API request to a language model with a Prompt.
- Direct LLM calls should include the relevant Prompt and Context for execution.

#### Instruction
- Instructions tell the agent how to behave and how to use its tools.
- Instructions may fulfill one or more Requirements.

#### Human Interaction
- Human interaction is a step requiring user input or oversight during agent execution.
- Human interactions may pause the agent until input is provided.
- Some human interactions can be passive, providing feedback without stopping execution.

#### Context
- Context consists of additional information injected into an Agent's prompt to situate it.
- Context can come from the Environment, Memory, or User input.
- Context may include Model settings or runtime parameters.

#### Output Schema
- An output schema defines the structure and validation rules for an agent’s output.
- Output schemas can be formally specified using structured languages (e.g., JSON Schema).

#### Prompt Template
- A prompt template is a reusable prompt structure with placeholders to fill in.
- Prompt templates can be predefined by the system or defined by Users.

#### Requirement
- A requirement is a condition or rule that controls when and how a tool will be used by an agent.
- Requirements may specify constraints or prerequisites for tool invocation.

#### Server
- A server provides external access to agent components or services via an API.
- Servers host the framework's interfaces (e.g., REST endpoints) for clients.

#### File
- File is a standard way to store and transfer external information.
- File may take different formats like Text, Audio, Video and more.
- Files may be stored in Memory or Storage, or converted to embeddings for retrieval.

#### Interpreter
- Interpreter might be a external computational system that computes something asked by the Agent
- Interpreter might execute generated code
- Interpreter might be configured as a sandbox

#### Runtime
- Runtime refers to the execution context of an agent or its components.
- A runtime environment can be an isolated interpreter (sandbox) or an external API.

#### KV Storage
- KV Storage (key-value storage) is a simple database for storing temporary data or cached information.
- KV Storage is often used for quick lookups or shared state in an agent workflow.

#### Node
- A node is a component or step within an agent's workflow.
- Nodes are connected by Transitions to form a workflow or decision graph.

#### Toolkit
- A toolkit is a collection of Tools available to Agents.
- Toolkits may provide shared resources (Memory, Storage, etc.) for their tools.

#### Embedding
- Embeddings are a low-level representation of information used by the Agent.
- Embeddings may be stored in Memory and Storage.
- Embeddings might be represented as vectors.

#### Step
- Steps might be defined by the User.
- Steps represent Transitions in a Workflow.

#### Transitions
- Transitions define conditions for moving between Steps in a Workflow.
- Transitions control the flow of execution from one Step to another in a Workflow.

