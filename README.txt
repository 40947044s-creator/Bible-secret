# Bible-LWE: Lattice-Based Inference Engine 📜🔏

A conceptual implementation of **Learning With Errors (LWE)** cryptography, treating the text of the Bible as a high-dimensional secret vector. This project explores the "Power of Three"—the triad of **Secret ($s$)**, **Transformation ($A$)**, and **Noise ($e$)**—to demonstrate how structured truth can be recovered from randomized interference.

---

## 🧩 The Concept

In this engine, we transform sacred text into binary machine code and treat it as a parameter in a noisy multiplication problem. The goal is to perform a **lattice inference** to "peel away" user-injected entropy and restore the original bitstring.

### The Mathematical Triad:
1.  **The Secret ($s$):** The Bible text converted into a binary vector.
2.  **The Matrix ($A$):** The structural operator that defines the lattice.
3.  **The Noise ($e$):** Randomized interference (seeded by user input) that obscures the secret.

**The Goal:** Recover $s$ from the noisy observation $b = As + e$.

---

## 🚀 Features

* **Binary Text-to-Vector Mapping:** Converts any string (defaulting to the Bible) into a processable binary format.
* **User-Injected Noise:** Allows manual perturbation of the lattice using custom text strings to seed the error distribution.
* **Rounding Inference:** A simulation of the Nearest Plane algorithm to resolve bit-level errors.
* **Real-time Visualization:** Dual-stream view comparing the "Pure" bitstream against the "Noisy" ciphertext.

---

## 🛠️ Usage

1.  **Input the Secret:** Paste a fragment of the Bible (or any text) into the Source Text area.
2.  **Inject Noise:** Provide a "Seed" string. The engine uses the entropy of your input to determine the weight and distribution of the error vector $e$.
3.  **Execute Inference:** The engine performs a parameter multiplication, adds your noise, and then attempts to solve the Shortest Vector Problem (SVP) logic to recover the text.

---

## 🔬 Cryptographic Context

This project is a simplified visualization of **Lattice-Based Cryptography**, specifically inspired by **2-adic LWE analysis** and **Project NP**. 

In a real-world LWE scenario, the "noise" is drawn from a Discrete Gaussian distribution. Here, we simulate that interference by perturbing the bit-coordinates of the text-vector, demonstrating that even when the "machine code" looks like randomized chaos, the underlying "Secret" remains invariant if the recovery parameters are known.

---

## 💻 Tech Stack

* **Frontend:** HTML5, CSS3 (Neon-Terminal Aesthetic)
* **Logic:** JavaScript (ES6+) bitwise operations and modular arithmetic.

---

> "One is an incident, two is a coincidence, three is a pattern." 
> — Making sense of the noise through the power of three.
