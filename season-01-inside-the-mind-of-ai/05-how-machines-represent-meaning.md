# Episode 05: How Machines Represent Meaning

> **Season 1: Inside the Mind of AI**  
> Instructor: **Akshay Saini** (NamasteDev)  
> Topic: How AI Understands Meaning, Polysemy, Why Token IDs Lack Meaning, Vectorization, and Dimensions

---

## 1. The Core Mystery: How Does AI Understand Meaning?

Consider the following statements:
1. "I ate an **apple** in the afternoon."
2. "**Apple** has launched a new device."

In human conversation, the distinction is immediate and effortless:
- In sentence 1, apple refers to a sweet edible fruit.
- In sentence 2, Apple refers to a multinational consumer technology corporation.

Another classic example:
1. "I am sitting near a river **bank**."
2. "I have a savings account in a **bank**."

One refers to sloping riverfront land, while the other refers to a licensed financial institution.

Human language is rich in **polysemy** (words possessing multiple distinct meanings depending on context), tone, nuance, and sarcasm. 

From first principles:
- Computers do not possess human cognition, eyes, or mental intuition.
- Natural Language Processing (NLP) must solve the fundamental challenge: how can a machine, which only operates on numbers, comprehend the true meaning and context behind words?

---

## 2. Why Token IDs Do Not Contain Any Meaning

In Episode 04, the text-to-token pipeline was established:
1. Sentences are segmented into discrete tokens by a tokenizer.
2. Each unique token is assigned an integer known as a **Token ID**.
3. The array of Token IDs is passed into the model.

However, a critical limitation exists: **Token IDs carry zero semantic meaning.**

<img src="../assets/season-01-inside-the-mind-of-ai/05-how-machines-represent-meaning/01-token-ids-do-not-contain-meaning-examples.png" alt="Token to Token ID Mapping Examples" width="600" />

Consider four sample tokens from a tokenizer vocabulary:

| Token | Token ID |
| :--- | :--- |
| **Dog** | `8123` |
| **Mango** | `612` |
| **Cat** | `123` |
| **Grapes** | `8521` |

If we hide the words and inspect only the numbers:
- `8123` (Dog) and `8521` (Grapes) are numerically close to each other.
- But Dog and Grapes share virtually no semantic relationship in the real world.
- Conversely, Dog and Cat are closely related animals, yet their Token IDs (`8123` and `123`) are distant.
- Mango and Grapes are both sweet fruits, yet their Token IDs (`612` and `8521`) are distant.

Token IDs are merely arbitrary, sequential integer identifiers assigned to tokens in a vocabulary lookup table. Numerical proximity of Token IDs does not indicate semantic similarity.

### The Student Roll Number Analogy

<img src="../assets/season-01-inside-the-mind-of-ai/05-how-machines-represent-meaning/02-token-ids-are-arbitrary-labels-roll-number-analogy.png" alt="Student Roll Number Analogy" width="600" />

Think of Token IDs like student roll numbers in a classroom:
- Student A has roll number `20`.
- Student B has roll number `22`.
- Student C has roll number `23`.
- Student D has roll number `45`.

Just because roll numbers `20` and `22` are adjacent numbers does not mean those two students are best friends, share identical skills, or have similar personalities. They are simply arbitrary administrative labels. The same principle applies to hotel room numbers: room `101` and room `102` do not indicate anything about the guests inside.

Because Token IDs are meaningless administrative labels, a model cannot rely on them alone to understand language or relationships.

---

## 3. What is Vectorization?

To give machines the ability to process meaning, information must undergo **Vectorization** (also spelled Vectorisation).

> **Vectorization is the process of converting information into numerical vectors (an array of numbers).**

<img src="../assets/season-01-inside-the-mind-of-ai/05-how-machines-represent-meaning/03-what-is-vectorization-converting-information-into-numerical-vectors.png" alt="What is Vectorization" width="600" />

Examples of numerical vectors:
- Two-dimensional vector: `[2, 5]`
- Three-dimensional vector: `[3, 8, 7]`
- Multi-dimensional vector: `[0.12, -3.5, 4.20, 1.24, -6.81]`

Any type of information can be vectorized:
- Text (words, sentences, documents)
- Images and visual scenes
- Audio and speech
- User profiles, products, or interactions

### Why Vectorization is Essential

Computers cannot perform mathematical operations on raw words or arbitrary ID tags. 

**Vectorization turns information into a mathematical format on which computers can perform mathematical operations.**

Once information is in vector form, linear algebra, geometry, dot products, and distance formulas can be applied to measure relationships, calculate similarity, and make predictions.

---

## 4. Representing Concepts via Dimensions: The Fruit Ranking Exercise

To understand how an array of numbers captures real-world meaning, consider an intuitive exercise: ranking fruits along three specific properties.

<img src="../assets/season-01-inside-the-mind-of-ai/05-how-machines-represent-meaning/04-ranking-fruits-on-dimensions-properties-to-vectors.png" alt="Ranking Fruits Across Three Dimensions" width="600" />

In mathematics and machine learning, each property is called a **Dimension**:
1. **Dimension 1**: Sweetness (scale from `0.0` to `1.0`)
2. **Dimension 2**: Size (scale from `0.0` to `1.0`)
3. **Dimension 3**: Crunchiness (scale from `0.0` to `1.0`)

Evaluating items across these three dimensions generates numerical vectors:

| Item | Sweetness | Size | Crunchiness | Resulting Vector |
| :--- | :--- | :--- | :--- | :--- |
| **Apple** | `0.7` | `0.4` | `0.8` | `[0.7, 0.4, 0.8]` |
| **Banana** | `0.8` | `0.6` | `0.2` | `[0.8, 0.6, 0.2]` |
| **Carrot** | `0.2` | `0.5` | `0.9` | `[0.2, 0.5, 0.9]` |
| **Watermelon** | `0.6` | `0.9` | `0.5` | `[0.6, 0.9, 0.5]` |

### How Vectors Reveal Meaning Mathematically

Notice what happens when concepts are translated into vectors:
- **Crunchiness**: If a machine searches for crunchy items, it inspects dimension 3: Apple (`0.8`) and Carrot (`0.9`) have high values, while Banana (`0.2`) has a low value.
- **Sweetness**: Banana (`0.8`) and Apple (`0.7`) share high sweetness values, grouping them closer together along that dimension.

Each number inside the vector is not random: it captures a specific attribute or feature of the object.

---

## 5. From Manual Properties to Learned Dimensions

In our three-fruit example, humans manually picked sweetness, size, and crunchiness. But human language contains millions of nuances, relationships, and concepts.

Modern embedding models operate on a vastly larger scale:
- Modern models do not use 3 dimensions. They use **thousands of dimensions** (for example, 768, 1536, or 3072 dimensions per vector).
- **Dimensions are not defined by humans**: Engineers do not manually assign scores or handcraft what each dimension represents.
- **Dimensions are learned automatically from data**: During training, the embedding model processes billions of sentences across internet texts, books, code, and articles.

### How Models Learn Dimensions Automatically

When a model reads vast corpora of text:
- The word "banana" repeatedly appears alongside phrases such as "sweet fruit", "yellow skin", "tropical peel", and "smooth texture".
- Each time the model processes these co-occurrences, mathematical training algorithms adjust and tune the numerical coordinates up or down.
- Over time, the model converges on stable numerical representations where words with related concepts naturally align closely in multi-dimensional space.
