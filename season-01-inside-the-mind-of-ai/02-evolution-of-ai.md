# Episode 02: Evolution of AI

> **Season 1: Inside the Mind of AI**  
> Instructor: **Akshay Saini** (NamasteDev)  
> Topic: The Complete Journey of AI: From Rule-Based Systems to Autonomous Agents

---

## 1. What Is Intelligence?

Before understanding Artificial Intelligence, we must first understand what **intelligence** itself means.

Intelligence is the ability to **acquire knowledge**, **process information**, **reason through problems**, and **adapt to new situations**. It is not limited to humans: animals, insects, and even plants demonstrate forms of intelligence.

![Evolution of AI Overview](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/01-evolution-of-ai-overview.jpg)

### Key Traits of Intelligence
- **Learning**: Gaining new knowledge from experience or instruction.
- **Reasoning**: Using logic to draw conclusions or make decisions.
- **Problem Solving**: Finding solutions to unfamiliar challenges.
- **Adaptation**: Adjusting behavior based on new inputs or environments.

---

## 2. Types of Intelligence

Intelligence is not a single, monolithic thing. It comes in different forms across different entities in nature.

### Categories
- **Human Intelligence (HI)**: The broadest form; includes language, abstract thinking, creativity, emotional reasoning, planning, and self-awareness.
- **Animal Intelligence**: Dogs can understand commands, dolphins communicate using patterns, and crows use tools; each species exhibits specialized intelligence.
- **Synthetic / Artificial Intelligence**: Intelligence demonstrated by machines. Systems that can perceive, learn, reason, and act, built and programmed by humans.

> [!NOTE]
> The term **"Synthetic Intelligence"** is sometimes used interchangeably with Artificial Intelligence. Both refer to machine-based intelligence designed to mimic or assist human cognitive abilities.

---

## 3. What Is Artificial Intelligence?

**Artificial Intelligence (AI)** is the science of building machines or software systems that can perform tasks which typically require human intelligence.

![What is Artificial Intelligence?](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/02-what-is-artificial-intelligence.jpg)

AI is a **broad umbrella term**. It covers everything from simple rule-based calculators to self-driving cars to ChatGPT. Any system that exhibits even basic forms of intelligence such as learning, reasoning, and decision-making falls under AI.

### Common Misconception
Many people think AI only means chatbots or Large Language Models. In reality, AI has existed for decades in many forms: spam filters, recommendation systems, chess engines, voice assistants, and more.

---

## 4. Evolution of AI: The Complete Timeline

This is the core of Episode 02. Akshay walks through the entire history of AI step by step, explaining how each era built on the limitations of the previous one.

### The Journey at a Glance

```
Rule-Based Systems → Machine Learning → Deep Learning → Transformers → LLMs → Agents
```

Each stage represents a fundamental shift in how machines learn and operate.

![AI Timeline Summary Board](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/16-ai-timeline-summary.jpg)

### Early Foundations: Turing Test and Dartmouth Conference (1950s)

In 1950, **Alan Turing** published his landmark paper proposing the famous **Turing Test** to explore the fundamental question: *"Can machines think?"*

In 1955-1956, **John McCarthy**, Marvin Minsky, Nathaniel Rochester, and Claude Shannon organized the Dartmouth Summer Research Project on Artificial Intelligence, formally coining the term **"Artificial Intelligence"** with the ambitious belief:

> *"Every aspect of learning and intelligence could, in principle, be described precisely enough for a machine to simulate it."*

![Early AI Foundations: Turing and McCarthy](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/03-early-ai-foundations-turing-mccarthy.jpg)

---

## 5. Rule-Based Systems (1950s-1980s)

The earliest form of AI. These systems operated entirely on **manually written if-else rules** defined by human experts.

![Rule-Based AI](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/04-rule-based-ai.jpg)

### How They Worked
- A human expert would define every possible scenario as a rule.
- The machine would follow these rules strictly with no learning and no adaptation.
- Example: A medical diagnosis system where a doctor writes rules like:  
  `IF fever > 102°F AND cough = true THEN diagnose = "flu"`

### Limitations
- **Rigid**: Could not handle scenarios not covered by the rules.
- **Not Scalable**: As the problem domain grew, the number of rules exploded.
- **No Learning**: The system never improved on its own. Every new scenario required a human to write a new rule.

### Real-World Examples
- Early chess programs (pre-Deep Blue era)
- Expert systems like MYCIN (medical diagnosis, 1970s)
- Basic spam filters using keyword matching

---

## 6. Machine Learning (1990s-2010s)

The breakthrough idea: instead of telling machines **what to do**, let them **learn from data**.

![Machine Learning](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/05-machine-learning.jpg)

### The Core Shift
- **Rule-Based**: Human writes rules → Machine follows rules.
- **Machine Learning**: Human provides data → Machine discovers patterns → Machine creates its own rules.

### How It Works
1. Provide the machine with a **large dataset** of input-output examples.
2. The algorithm finds **statistical patterns** in the data.
3. Based on these patterns, the machine builds a **model** that can make predictions on new, unseen data.

### Types of Machine Learning
| Type | Description | Example |
| :--- | :--- | :--- |
| **Supervised Learning** | Learns from labeled data (input + correct output) | Email spam detection |
| **Unsupervised Learning** | Finds hidden patterns in unlabeled data | Customer segmentation |
| **Reinforcement Learning** | Learns by trial and error with rewards/penalties | Game-playing AI |

### Limitations
- Required **feature engineering**: Humans still had to manually select which data features to feed the model.
- Struggled with unstructured data like images, audio, and natural language.
- Performance plateaued on complex tasks.

---

## 7. Deep Learning (2010s)

Deep Learning is a **subset of Machine Learning** that uses **neural networks** with multiple layers to automatically learn features from raw data.

![Deep Learning](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/06-deep-learning.jpg)

### Why "Deep"?
The word "deep" refers to the **depth** of the neural network, meaning the number of hidden layers between the input and output. More layers allow the network to learn increasingly **abstract and complex representations**.

### Machine Learning vs Deep Learning

![Machine Learning vs Deep Learning](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/07-machine-learning-vs-deep-learning.jpg)

### What Changed
- **No more manual feature engineering**: The network automatically discovers relevant features.
- **Handles unstructured data**: Images, audio, video, and text can be processed directly.
- **Powered by GPUs**: Graphics Processing Units made training deep networks computationally feasible.

---

## 8. Neural Network Structure

A neural network is inspired by the human brain. It consists of layers of interconnected nodes (neurons) that process information.

### Architecture
- **Input Layer**: Receives the raw data (pixels, words, numbers).
- **Hidden Layers**: Process and transform the data through weighted connections. Each layer extracts higher-level features.
- **Output Layer**: Produces the final prediction or classification.

### Key Concepts
- **Weights**: Numerical values on connections that the network adjusts during training.
- **Activation Functions**: Mathematical functions that determine whether a neuron "fires" or not.
- **Backpropagation**: The algorithm that adjusts weights based on the error between predicted and actual output.

---

## 9. Deep Neural Networks

When a neural network has **many hidden layers** (often dozens or hundreds), it is called a **Deep Neural Network (DNN)**.

### Why Depth Matters
Each layer in a deep network learns a different level of abstraction:

| Layer Depth | What It Learns (Image Example) |
| :--- | :--- |
| **Early layers** | Edges, lines, basic shapes |
| **Middle layers** | Textures, patterns, parts of objects |
| **Deep layers** | Full objects, faces, scenes |

### Breakthroughs Powered by Deep Learning: The Computer Vision Revolution

In 2012, **AlexNet** won the ImageNet competition using a deep convolutional neural network, slashing error rates and triggering the modern deep learning boom.

![Computer Vision Revolution: AlexNet](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/08-computer-vision-alexnet.jpg)

### Key Breakthrough Areas
- **Image Recognition**: CNNs (Convolutional Neural Networks) surpassed human accuracy on ImageNet (2015); enabled face unlock, self-driving perception, and automated medical imaging.
- **Speech Recognition**: Siri, Google Assistant, Alexa.
- **Natural Language Processing**: Early translation and sentiment classification.
- **Game Playing**: AlphaGo defeating the world champion in Go (2016).

---

## 10. The AI Winter

Not everything was smooth progress. AI went through periods called **"AI Winters"**, times when funding dried up, hype collapsed, and progress stalled.

### What Caused AI Winters?
- **Overpromising and Underdelivering**: Early researchers promised human-level AI within decades. When that did not happen, governments and corporations pulled funding.
- **Computational Limitations**: The hardware of the time simply could not support the algorithms researchers had designed.
- **Limited Data**: Modern AI thrives on massive datasets. In earlier decades, data was scarce and expensive to collect.

### Timeline
| Period | Event |
| :--- | :--- |
| **1st AI Winter (1974-1980)** | DARPA cut funding after early AI systems failed to scale |
| **2nd AI Winter (1987-1993)** | Expert systems proved too brittle for real-world use |
| **The Revival (2012+)** | Deep learning + big data + GPUs reignited the field |

> [!IMPORTANT]
> The AI winters teach us an important lesson: **hype without substance does not last**. The current AI boom is powered by real, measurable capabilities, but it is crucial to keep expectations grounded.

---

## 11. Transformers: The Architecture That Changed Everything (2017)

The **Transformer architecture** is the single most important innovation in modern AI. It was introduced in the landmark paper **"Attention Is All You Need"** by Vaswani et al. at Google in 2017.

### The Pre-Transformer Era: Natural Language Processing and RNNs

Before Transformers, Natural Language Processing relied on methods like Bag of Words, n-grams, and sequential models like RNNs (Recurrent Neural Networks) and LSTMs (Long Short-Term Memory networks). These models processed text **one word at a time**, making them slow and unable to handle long-range dependencies effectively.

![Natural Language Processing and RNNs](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/09-natural-language-processing-nlp.jpg)

### What Made Transformers Special?
Transformers introduced the **Self-Attention Mechanism**, which allows the model to look at **all words in a sentence simultaneously** and determine which words are most relevant to each other.

![Transformers: Attention Is All You Need](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/10-transformers-attention-is-all-you-need.jpg)

### Key Advantages
- **Parallelization**: Unlike RNNs, Transformers process all tokens at once, making training dramatically faster.
- **Long-Range Context**: The attention mechanism can relate words that are far apart in a sentence.
- **Scalability**: Transformers scale efficiently with more data and compute, enabling the training of billion-parameter models.

---

## 12. "Attention Is All You Need": The Paper

This 2017 paper from Google is considered the **foundational paper of modern AI**. It introduced the Transformer architecture that powers every major AI model today.

### Why It Matters
- Replaced RNNs and LSTMs as the dominant architecture for NLP.
- Became the backbone of GPT, BERT, T5, LLaMA, Gemini, Claude, and virtually every major language model.
- The concept of **"Attention"**, letting the model decide what to focus on, turned out to be the key breakthrough for understanding language at scale.

> [!TIP]
> If you want to deeply understand modern AI, reading and understanding this paper (even at a high level) is extremely valuable. Akshay covers this in detail in later episodes.

---

## 13. Large Language Models (LLMs)

A **Large Language Model** is a Transformer-based model trained on **massive amounts of text data** to understand and generate human language.

![Large Language Models](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/11-large-language-models-llms.jpg)

### What Makes an LLM "Large"?
- **Parameters**: LLMs have billions (sometimes trillions) of trainable parameters (weights). GPT-3 had 175 billion parameters. GPT-4 is estimated to have over a trillion.
- **Training Data**: Trained on vast corpora of text, including books, websites, code, scientific papers, and conversations.
- **Compute**: Training an LLM requires thousands of GPUs running for weeks or months.

### How LLMs Work (Simplified)
1. The model reads a sequence of text (prompt).
2. Using its learned patterns, it **predicts the next most likely token** (word or subword).
3. It generates text one token at a time, each prediction building on the previous output.

### Generative AI: From Analysis to Generation

Earlier AI was primarily discriminatory: classifying, predicting numbers, or recommending products. Large Language Models enabled **Generative AI**, creating new text, code, audio, and multimodal artifacts.

![Generative AI](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/12-generative-ai.jpg)

---

## 14. The GPT Journey

**GPT (Generative Pre-trained Transformer)** is the model family by OpenAI that brought LLMs into the mainstream.

### Evolution of GPT

| Model | Year | Parameters | Key Milestone |
| :--- | :--- | :--- | :--- |
| **GPT-1** | 2018 | 117 Million | Proved that pre-training + fine-tuning works |
| **GPT-2** | 2019 | 1.5 Billion | Generated coherent long-form text; OpenAI initially withheld it due to misuse concerns |
| **GPT-3** | 2020 | 175 Billion | Few-shot learning; could perform tasks with minimal examples |
| **GPT-3.5** | 2022 | ~175 Billion | Fine-tuned with RLHF (Reinforcement Learning from Human Feedback); powered the initial ChatGPT |
| **GPT-4** | 2023 | ~1.7 Trillion (estimated) | Multimodal (text + images); significantly improved reasoning |
| **GPT-4o** | 2024 | Undisclosed | Omni-model: native text, audio, and vision capabilities |

### The Multimodal Shift: GPT-4o and Beyond

Modern AI models are no longer confined to text alone. Multimodal AI models seamlessly understand and generate content across images, voice, video, code, and documents.

![Multimodal AI](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/14-multimodal-ai.jpg)

---

## 15. The ChatGPT Moment

**ChatGPT**, launched on November 30, 2022, became the **fastest-growing consumer application in history**, reaching 100 million users in just 2 months.

![The ChatGPT Moment](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/13-chatgpt-moment.jpg)

### Why Was It a Watershed Moment?
- **Accessible to Everyone**: For the first time, a powerful AI model was available through a simple chat interface that anyone could use.
- **Proved LLMs Work**: Demonstrated that LLMs could hold coherent conversations, write code, create content, and reason through problems.
- **Triggered the AI Race**: Every major tech company (Google, Meta, Anthropic, Microsoft) accelerated their AI efforts.
- **Changed Industries**: Software development, content creation, education, healthcare, legal; every sector started exploring AI integration.

> [!NOTE]
> ChatGPT was not the most advanced model technically. Its success came from making powerful AI **accessible** and **usable** through a simple conversational interface.

---

## 16. Top AI Companies and the AI Race

The launch of ChatGPT triggered an unprecedented race among technology companies to build and deploy LLMs.

### Major Players

| Company | Key Model(s) | Notable Contribution |
| :--- | :--- | :--- |
| **OpenAI** | GPT-4, GPT-4o, o1 | Pioneered the LLM revolution with ChatGPT |
| **Google DeepMind** | Gemini, PaLM, AlphaFold | Multimodal AI, protein structure prediction |
| **Anthropic** | Claude 3.5, Claude 4 | Focus on AI safety and constitutional AI |
| **Meta** | LLaMA 3, Code LLaMA | Open-source LLMs democratizing AI access |
| **Microsoft** | Copilot, Phi | Deep integration of AI into productivity tools |
| **xAI (Elon Musk)** | Grok | Real-time information access |
| **Mistral** | Mixtral, Mistral Large | High-performance open-weight European models |

### The Compute Arms Race
- Training frontier models costs **hundreds of millions of dollars**.
- Companies are building massive GPU clusters (10,000+ NVIDIA H100s).
- The race is not just about model quality but also about **speed, cost, and accessibility**.

---

## 17. AI Agents: The Next Frontier

An **AI Agent** is an LLM-powered system that can **autonomously plan, reason, use tools, and take actions** to accomplish complex tasks.

Earlier AI could only answer questions in single-turn conversations. Today, modern AI systems can think, plan, call APIs, write code, search the web, and use tools to perform end-to-end work.

![The AI Today: Tool Use and Capabilities](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/15-the-ai-today-capabilities.jpg)

### From Chatbots to Agents
| Feature | Chatbot (LLM) | AI Agent |
| :--- | :--- | :--- |
| **Interaction** | Single turn Q&A | Multi-step autonomous workflows |
| **Tool Use** | None | Can call APIs, search the web, run code |
| **Planning** | None | Breaks complex tasks into sub-tasks |
| **Memory** | Limited to context window | Maintains state across sessions |
| **Action** | Generates text | Executes real-world actions |

### How Agents Work
1. **Receive a Goal**: The user defines a high-level objective.
2. **Plan**: The agent breaks the goal into a sequence of steps.
3. **Execute**: The agent uses tools (APIs, code execution, web search) to complete each step.
4. **Reflect**: The agent evaluates its output and adjusts if needed.
5. **Iterate**: The loop continues until the goal is achieved.

### Examples of AI Agents
- **Coding Agents**: Devin, GitHub Copilot Workspace, Cursor Agent
- **Browser Agents**: Agents that navigate the web autonomously
- **Research Agents**: Agents that read papers, summarize findings, and generate reports

---

## 18. AlphaGo: The Defining Moment for AI

Akshay references the **AlphaGo documentary**, a pivotal moment in AI history that proved machines could master tasks previously thought to be uniquely human.

### The Story
- **Go** is an ancient board game with more possible positions than atoms in the universe (~10^170 positions). It was considered the "holy grail" of AI game-playing.
- In **March 2016**, **AlphaGo** (by Google DeepMind) defeated **Lee Sedol** (one of the greatest Go players of all time) 4-1 in a five-game match.
- AlphaGo used a combination of **deep neural networks** and **reinforcement learning**. It learned by playing millions of games against itself.

### The Legendary Move 37

In Game 2 against Lee Sedol, AlphaGo played **Move 37**, a move that shocked Go masters around the world. No human player would have played it; commentators initially called it a mistake, but it turned out to be a stroke of creative genius that completely altered the trajectory of the game.

![Move 37: Lee Sedol vs AlphaGo](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/17-alphago-move-37.jpg)

### Why It Matters
- Proved that AI could handle **intuition-based** tasks, not just brute-force calculation.
- Lee Sedol himself said AlphaGo made moves that no human would ever think of: creative, unconventional, and brilliant.
- This event inspired a generation of AI researchers and engineers.

### Recommended Documentary: AlphaGo - The Movie

![AlphaGo Documentary](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/18-alphago-documentary.jpg)

> [!TIP]
> Akshay highly recommends watching the **"AlphaGo - The Movie"** documentary (available on YouTube for free by Google DeepMind). It is an inspiring watch for anyone entering the AI field.

---

## 19. Where Is the Industry Going?

Akshay outlines the key trends and technologies that are shaping the future of AI.

![Where is the Industry Going?](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/19-where-is-the-industry-going.jpg)

### Future Directions
- **Agentic AI**: Autonomous systems that plan, reason, and execute multi-step tasks.
- **Multimodal AI**: Models that natively understand text, images, audio, and video together.
- **Multi-Agent Orchestration**: Multiple AI agents collaborating to solve complex problems.
- **Reasoning Models**: Models specifically trained for logical, mathematical, and scientific reasoning (e.g., OpenAI o1).
- **RAGs (Retrieval-Augmented Generation)**: Combining LLMs with external knowledge bases for accurate, up-to-date responses.
- **MCP / OKF**: Protocols for standardizing how AI models interact with tools and context.
- **Robotics**: AI-powered robots performing physical tasks in the real world.
- **Every Possible Industry**: AI is expanding into healthcare, finance, education, agriculture, manufacturing, legal, and beyond.

---

## 20. Robotics: AI in the Physical World

Akshay showcases real-world examples of AI-powered robotics to illustrate how far the technology has come.

![Robotics: Chinese Spring Festival Search](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/20-robotics-chinese-spring-festival.jpg)

### Humanoid Martial Arts Performance

At the **2026 Chinese Spring Festival Gala**, humanoid robots performed synchronized **martial arts and dance routines** on stage alongside human performers.

![Martial Arts Robots at Spring Festival Gala](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/21-martial-arts-robots.jpg)

### Highlights
- These robots demonstrated real-time balance, coordination, and movement planning, all powered by AI.
- This is a glimpse of **embodied AI**, intelligence that exists not just in software but in physical machines that interact with the real world.

---

## 21. What Namaste AI Will Cover

The episode concludes with Akshay revisiting the **five pillars** of what Namaste AI will teach:

![Namaste AI Course Pillars](../assets/season-01-inside-the-mind-of-ai/02-evolution-of-ai/22-namaste-ai-course-pillars.jpg)

### The Five Pillars
1. **Foundational Knowledge**: Core concepts, history, and mental models of AI.
2. **Basic Building Blocks**: Tokens, embeddings, attention, context windows, prompts.
3. **What is Relevant Today**: Current state of LLMs, tools, and industry practices.
4. **Tools and Projects**: Hands-on building with real tools and end-to-end projects.
5. **Practical Aspect of AI**: Real-world applications, deployment, evaluation, and optimization.

---

## Summary: The Evolution at a Glance

| Era | Period | Key Idea | Limitation |
| :--- | :--- | :--- | :--- |
| **Rule-Based Systems** | 1950s-1980s | Human writes explicit rules | Rigid, not scalable, no learning |
| **Machine Learning** | 1990s-2010s | Machine learns patterns from data | Requires manual feature engineering |
| **Deep Learning** | 2010s | Neural networks auto-learn features | Needs massive data and compute |
| **Transformers** | 2017+ | Attention mechanism, parallel processing | Still needs huge compute |
| **Large Language Models** | 2020+ | Billion-parameter models understand language | Hallucinations, context limits |
| **AI Agents** | 2024+ | Autonomous planning, tool use, multi-step execution | Early stage, reliability challenges |

---

## Summary Checklist

- Understand what intelligence is and its different types (human, animal, synthetic).
- Know the complete evolution timeline: Rule-Based → ML → Deep Learning → Transformers → LLMs → Agents.
- Understand why rule-based systems failed and how machine learning solved it.
- Know what neural networks and deep neural networks are and why depth matters.
- Understand the significance of the Transformer architecture and the "Attention Is All You Need" paper.
- Know what Large Language Models are and how they generate text.
- Trace the GPT journey from GPT-1 (117M params) to GPT-4o.
- Understand why ChatGPT was a watershed moment for AI accessibility.
- Know the major players in the AI race and their key contributions.
- Understand what AI Agents are and how they differ from simple chatbots.
- Be aware of where the industry is heading: Agentic AI, Multimodal, Reasoning Models, Robotics, and more.

---

## Additional Information: Sources Beyond the Course

The following information was added from external research and other student discussions to supplement the course content:

1. **"Attention Is All You Need" Paper Details**: The paper was authored by Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez, Lukasz Kaiser, and Illia Polosukhin. It was published at NeurIPS 2017. The specific architectural details (self-attention mechanism replacing RNNs) and the impact on subsequent model development were supplemented from the original paper and public research summaries.

2. **GPT Parameter Counts**: Exact parameter counts for GPT-1 (117M), GPT-2 (1.5B), and GPT-3 (175B) are from published OpenAI papers. The estimated GPT-4 parameter count (~1.7 trillion, mixture-of-experts) is based on widely reported industry estimates and has not been officially confirmed by OpenAI.

3. **AI Winter Timeline**: The specific dates and causes of the two AI winters (1974-1980 and 1987-1993) were cross-referenced with the Wikipedia "AI Winter" article and the textbook by Stuart Russell and Peter Norvig, *"Artificial Intelligence: A Modern Approach"*.

4. **AlphaGo Match Details**: The March 2016 match result (4-1 victory over Lee Sedol) and the number of possible Go positions (~10^170) are from published Google DeepMind research and the AlphaGo documentary.

5. **ChatGPT Growth Statistics**: The "100 million users in 2 months" figure is from a UBS research report published in February 2023, widely cited across Reuters and other major publications.

6. **Spring Festival Gala 2026 Robots**: The martial arts robot performance at the Chinese Spring Festival Gala was widely covered by CGTN and international media in early 2026.

> [!NOTE]
> All core concepts, explanations, analogies, and the narrative flow in these notes are directly from the **Namaste AI Episode 02 lecture by Akshay Saini**. The supplementary information listed above only adds specific dates, numbers, and historical context to enhance accuracy.
