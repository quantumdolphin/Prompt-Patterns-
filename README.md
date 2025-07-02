# 🔧 Prompt Engineering Patterns: My Working Notebook

*My personal reference guide with tested prompts and examples*

---

## 🧠 Overview

This is my personal prompt engineering reference inspired by the [Prompt Engineering for ChatGPT](https://www.coursera.org/learn/prompt-engineering) course. It documents prompt patterns I've studied and applied — along with my own custom examples and use cases. Each section contains:

* A **prompting pattern**
* A **brief explanation**
* A **custom prompt I wrote**
* A **sample output** from ChatGPT

The goal is to turn this into a regular practice: crafting reusable prompt templates for real-world tasks in research, writing, analysis, and more.

---

## 🎮 1. Game Play Pattern

**🔹 What it is:**
This pattern creates a playful, role-based interaction — where the model pretends to be part of a fictional or goal-oriented game scenario.

**📝 Prompt:**

> You are a structural biologist in a simulation game. You receive data from cryo-EM, NMR, and X-ray crystallography. Your task is to identify which protein model is most likely correct. Clue 1: The resolution of Model A is 2.1 Å. Model B shows a flexible loop not present in others. What do you think?

**💬 Sample Output:**

> Based on Clue 1, Model A offers high resolution and likely accurate global features. However, the flexible loop in Model B suggests alternate conformational states. I would examine electron density maps further, but initially favor Model A for structure-based drug design.

**💡 Use Case:** Engaging educational scenarios, simulations, storytelling, creative ideation.

---

## 🧾 2. Template Pattern

**🔹 What it is:**
A structured format that ensures the model fills out predefined fields. Great for consistency and clarity in outputs.

**📝 Prompt Example (Applied to AlphaFold 3 Article):**

> Please provide a summary of the following article using this template:
> Title: \[Title]
> Developer: \[Developer]
> Main Advancement: \[Main technical or scientific advancement]
> Applications: \[What new things it can be used for]
> Access Model: \[How researchers can use it]

**🧪 Input Article Snippet:**
AlphaFold 3 was released in 2024 by DeepMind. It can now model protein–RNA, protein–ligand, and protein–DNA interactions with improved accuracy…

**💬 Sample Output:**

```
Title: AlphaFold 3 Expands Protein Structure Prediction
Developer: Google DeepMind
Main Advancement: Predicts protein-ligand and nucleic acid interactions with 50% more accuracy.
Applications: Drug design, RNA structure prediction, gene regulation.
Access Model: Not open-source, but available via DeepMind web server.
```

---

## 🧠 3. Meta Language Creation Pattern

**🔹 What it is:**
This pattern invents a domain-specific “meta language” that simplifies technical discussions using metaphorical or shorthand terminology. In drug design, terms like **“gatekeeper,” “molecular glue,” “hot spot,”** or **“cryptic pocket”** are widely used to convey complex ideas more intuitively.

**📝 Custom Prompt (Drug Design Domain):**

> We will use well-accepted metaphorical terms commonly used in medicinal chemistry and structural biology to describe kinase drug resistance. Use the following shorthand in your explanation:
>
> * “Gatekeeper” = residue that controls access to the back pocket of the kinase active site
> * “Hydrophobic spine” = key structural motif needed for kinase activation
> * “Molecular brake” = residues that stabilize the inactive conformation
> * “Switch pocket” = region that toggles between active and inactive states
> * “Water network” = conserved water molecules critical for ligand binding
>   Now, explain why a T670V gatekeeper mutation in KIT can cause resistance to a type II inhibitor.

**💬 Sample Output:**

The T670V mutation in KIT alters the **gatekeeper** residue, which normally regulates access to the deep hydrophobic pocket targeted by type II inhibitors. When threonine is replaced by valine, the entrance to this pocket becomes narrower and more hydrophobic, disrupting access to the **switch pocket** and weakening key contacts. This shift also disrupts the **water network** that typically helps anchor the inhibitor. As a result, the drug can no longer stabilize the **molecular brake**, making it harder to lock the kinase in its inactive state — leading to resistance.

---

## 🔀 5. Alternative Approaches Pattern

**🔹 What it is:**
Generates multiple strategies or perspectives to solve a problem. Useful in brainstorming and decision-making.

**📝 Prompt:**

> What are three different approaches to improve team collaboration in a remote work environment? Provide a brief description of each.

**💬 Sample Output:**

1. **Daily Standups:** Schedule short video calls each morning for team updates and alignment.
2. **Shared Digital Whiteboards:** Use tools like Miro to collaborate visually and asynchronously.
3. **Virtual Watercooler:** Schedule casual Zoom time or Slack channels for non-work banter to maintain team cohesion.

---

## 🔁 8. Few-Shot Learning Pattern

**🔹 What it is:**
Provides the model with **a few examples** so it can learn the expected format before completing a similar task.

**📝 Prompt:**

> Convert scientific abstracts into plain language.
>
> Example 1:
> Abstract: "The compound inhibited EGFR phosphorylation in a dose-dependent manner, reducing downstream signaling."
> Plain: "The drug blocked the EGFR protein, which helps stop the signal inside the cell."
>
> Example 2:
> Abstract: "Binding affinity was measured using isothermal titration calorimetry."
> Plain: "We tested how tightly two molecules stick using a heat-based experiment."
>
> Now simplify this:
> Abstract: "The kinase domain showed increased stability upon ligand binding, as confirmed by thermal shift assays."

**💬 Sample Output:**

> Plain: The protein became more stable when the drug attached to it. We confirmed this using a heat-based test.

---

## 🧩 9. Few-Shot + Sub-Steps Pattern

**🔹 What it is:**
A variation of few-shot prompting that includes intermediate reasoning steps to complete a complex task.

**📝 Prompt:**

> Here are two examples of breaking a research question into steps:
>
> Example 1:
> Question: How do kinase inhibitors overcome resistance in EGFR mutations?
> Step 1: Identify the mutation site.
> Step 2: Determine conformational effect.
> Step 3: Analyze inhibitor fit.
> Step 4: Compare IC50 or ΔG values.
>
> Example 2:
> Question: How does loop flexibility affect docking accuracy?
> Step 1: Identify loop region.
> Step 2: Assess flexibility via RMSF or B-factor.
> Step 3: Evaluate clashes in docking poses.
> Step 4: Re-dock with flexible constraints.
>
> Now try: How does water-mediated interaction impact ligand binding?

**💬 Sample Output:**

> Step 1: Identify water molecules forming bridges.
> Step 2: Assess their conservation across structures.
> Step 3: Evaluate their energetic contribution via MM-GBSA or MD analysis.
> Step 4: Compare binding modes with and without water.

---

*Sections 10–15 follow in the next update.*
