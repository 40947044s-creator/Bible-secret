# Project NP: NIV Bible Inference & Noise Extraction 📜⚡

> "Assuming there is noise in the Word, we treat the scripture as the ciphertext and the truth as the hidden signal."

This repository contains an experimental **NP-Inference Engine** that treats the **New International Version (NIV) Bible** as an encrypted medium. By connecting to a live Bible API, the engine processes the text as a **Noisy Ciphertext ($b$)** and attempts to recover a **Secret Bitstring ($s$)** through randomized error extraction.

---

## 🧩 The Core Philosophy: "Noise in the Word"

In traditional cryptography, the Bible is often used as the *Secret*. In **Project NP**, we reverse this:
1.  **The Bible ($b$):** The observable, public text (NIV).
2.  **The Noise ($e$):** The linguistic and historical "perturbations" inherent in the text.
3.  **The Secret ($s$):** The underlying machine-code bitstring discovered through inference.

We assume the relationship:  
$$b = s \cdot \text{Parameters} + e$$  
Our goal is to resolve the **Shortest Vector Problem (SVP)** to see what lies beneath.

---

## 🚀 System Features

* **Live Stream Decoding:** Real-time side-by-side view of the NIV source text and the extracted secret bitstring.
* **NP-Inference Logic:** A randomized decoding algorithm that treats ASCII/UTF-8 coefficients as noisy parameters.
* **Halt & Regenerate:** A manual override allowing the user to kill the current process, re-randomize the noise distribution (the Gaussian "Error"), and start a new inference cycle.
* **Gibberish Acceptance:** Adheres to the "Spirit of Extraction"—if the decoded secret is non-human-readable, it is accepted as a valid (yet unkeyed) mathematical result.

---

## 🛠️ Usage

1.  **Initialize:** Open the HTML interface to begin the API handshake.
2.  **Extraction:** Click `Begin Extraction` to start the live stream. The system will pull verses and immediately attempt noise removal.
3.  **Observation:** Watch the "Inferred Secret" panel. If a pattern emerges, the inference parameters are nearing the "Trapdoor."
4.  **Halt:** If the result is unsatisfactory, use the `Halt & Regenerate` button to reset the random seed and attempt a different lattice reduction.

---

## 🔬 Technical Context (LWE & 2-adic Analysis)

This project is part of a broader study into **Lattice-Based Cryptography** and **Learning With Errors (LWE)**. It explores how high-entropy texts (like the Bible) behave when subjected to p-adic carry-over analysis and modular reduction.

**Project NP** is an exploration of the boundary between information theory and theology—searching for a signal where most only see a story.

---

*Developed for algorithmic research at NTNU 資工系.*
https://40947044s-creator.github.io/Bible-secret/
