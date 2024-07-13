### Choice Blindness

**Choice blindness** is a cognitive phenomenon where individuals fail to notice discrepancies between their intended choices and the outcomes they are presented with, often rationalizing or confabulating reasons for the choices they did not actually make. This phenomenon reveals significant insights into the nature of decision-making, self-awareness, and introspection.

#### Key Aspects

1. **Definition**:
   Choice blindness refers to the failure to detect a mismatch between one's intended choice and the actual outcome, leading individuals to unknowingly accept and rationalize outcomes they did not choose.

2. **Origins**:
   The term was coined by Petter Johansson and colleagues in a series of experiments conducted in the early 2000s. Their research demonstrated that people often do not notice when their choices are manipulated, and they provide justifications for these non-chosen outcomes as if they were their original choices.

3. **Mechanisms**:
   - **[[Post-Choice Rationalization]]**: After making a choice, individuals generate reasons to support their decision, even if the outcome is not what they originally chose.
   - **[[Memory Reconsolidation]]**: People's memory of their choice can be altered to fit the presented outcome, leading them to believe the manipulated choice was their actual choice.
   - **Attention and Awareness**: Limited attention and awareness during the decision-making process can contribute to choice blindness, as discrepancies go unnoticed.

#### Experimental Evidence

**Johansson et al. (2005) Experiment**:
   - **Setup**: Participants were shown pairs of faces and asked to choose the more attractive one. Through sleight of hand, the experimenters sometimes presented the non-chosen face as the chosen one.
   - **Results**: A significant number of participants did not detect the switch and provided explanations for why they chose the face they had actually rejected.

**Additional Experiments**:
   - Similar experiments have been conducted with other types of choices, such as selecting consumer products, moral judgments, and political opinions, all showing that people often fail to detect changes and rationalize the manipulated outcomes.

#### Implications

1. **Decision-Making**:
   - **Consumer Behavior**: Understanding choice blindness can help marketers and product designers anticipate how consumers might justify their choices, even when they are not fully aware of their preferences.
   - **Voting and Political Opinions**: In the context of political decisions, choice blindness suggests that voters might be less aware of the inconsistencies in their stated preferences and actual choices.

2. **Self-Awareness**:
   - **Introspection**: The phenomenon challenges the reliability of introspection and self-reported data, as people may not be fully aware of their true preferences and the reasons behind their choices.
   - **Therapy and Counseling**: Recognizing choice blindness can be valuable in therapeutic settings, helping individuals understand the potential discrepancies between their perceived and actual preferences.

3. **Cognitive Psychology**:
   - **Memory and Attention**: Choice blindness highlights the malleability of memory and the role of attention in detecting and responding to changes in one's environment.

#### Mathematical Formalization

To formalize choice blindness, consider a decision-making model with two stages: choice and outcome presentation.

1. **Choice Stage**:
   Let $C$ represent the true choice made by an individual among options $O_1, O_2, \ldots, O_n$. Suppose $P(C = O_i)$ represents the probability of choosing option $O_i$.

2. **Outcome Presentation Stage**:
   Let $M$ represent the manipulated outcome presented to the individual, which may differ from $C$. Define $D$ as a binary variable indicating detection of the manipulation:
   $$
   D = 
   \begin{cases} 
   1 & \text{if the individual detects the manipulation} \\
   0 & \text{if the individual does not detect the manipulation}
   \end{cases}
   $$

   The probability of detecting the manipulation can be expressed as:
   $$
   P(D = 1) = f(\Delta),
   $$
   where $\Delta$ is the degree of discrepancy between $C$ and $M$, and $f(\Delta)$ is a function capturing the likelihood of detection, typically increasing with larger $\Delta$.

#### Experimental Design and Results Analysis

In experiments, the detection rate $P(D = 1)$ is often found to be surprisingly low, even when $\Delta$ is significant. This can be modeled by adjusting the function $f(\Delta)$ to reflect empirical findings, showing that individuals are prone to overlooking discrepancies and rationalizing non-chosen outcomes.

### Related Concepts

- [[Cognitive Bias]]
- [[Introspection Illusion]]
- [[Confirmation Bias]]
- [[Memory Reconsolidation]]

Understanding choice blindness is crucial for comprehending the limitations of human decision-making and the malleability of our preferences and justifications. This phenomenon underscores the importance of designing decision-making environments that account for these cognitive biases.