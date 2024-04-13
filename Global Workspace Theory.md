[[Global Workspace Theory|Global Workspace Theory (GWT)]] is a cognitive architecture theory proposed by Bernard Baars in the 1980s. It provides a framework for understanding [[consciousness]], particularly how information becomes conscious. The theory likens consciousness to a theater, where the spotlight of attention illuminates the central stage of working memory, making information globally available to a variety of specialized, unconscious processors in the brain.

### Key Concepts

- **Global Workspace (GW):** This is the central stage or "theater" where information is broadcasted to multiple specialized processes. Information that reaches the GW becomes accessible to conscious awareness, allowing for serial processing of information that is globally available across different brain modules.

- **Specialized Unconscious Processors:** These are akin to the audience or the backstage crew in the theater analogy. They operate outside of conscious awareness, processing specific types of information (e.g., visual, auditory, language). When they have information deemed important (through competition or relevance), it is pushed into the global workspace for conscious processing.

- **Conscious versus Unconscious Processing:** In GWT, consciousness arises from the global availability of information. This means that while many processes occur outside of conscious awareness, only information that wins the competition for attention and is broadcasted in the GW becomes part of conscious experience.

- **Attention and Working Memory:** Attention acts as a spotlight, highlighting information for global broadcast. Working memory serves as the stage of the GW, maintaining information in an easily accessible state for various cognitive processes.

### Mathematical Formalism

Let's formalize some of the theory's aspects using mathematical notation:

- **Global Workspace Dynamics:** Let's denote the set of all possible information pieces by $I$. A subset of this, $I_w \subset I$, represents information within the workspace at any given time. The dynamics of the global workspace can be modeled as a function $f$ that updates the state of the workspace based on new information, previous state, and feedback from specialized processors:

$$I_{w}^{t+1} = f(I_w^t, I_{new}, feedback)$$

- **Information Competition:** Information from unconscious processors competes for access to the global workspace. This can be represented by a competition function $C$, which takes as input information $I_{new}$ from processors and their respective weights or importance $w_i$:

$$I_{selected} = C(\{(I_{new,i}, w_i)\})$$

Here, $I_{selected}$ is the information that wins the competition and is broadcasted to the GW.

- **Conscious Access and Broadcast:** Once information is selected for the global workspace, it is broadcasted globally, affecting various unconscious processors. This can be modeled as a broadcasting function $B$, where:

$$B(I_{selected}) = \{effect\_on\_processor_j\}_{j=1}^{N}$$

where $N$ is the number of specialized processors influenced by the broadcast.

### Philosophical Implications

[[Global Workspace Theory|GWT]] has profound implications for the [[Philosophy of Mind|philosophy of mind]], particularly in discussions about the nature of consciousness, the hard problem of consciousness, and the functional role of conscious processing. It provides a framework for understanding how and why certain pieces of information become part of our conscious experience and how this process influences our decision-making, problem-solving, and creativity.

In summary, GWT offers a compelling model for understanding consciousness through the metaphor of a global workspace, highlighting the interplay between conscious and unconscious processing and the central role of attention and working memory in consciousness.