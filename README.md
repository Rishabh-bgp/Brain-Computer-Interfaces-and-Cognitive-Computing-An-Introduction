# Brain–Computer Interfaces and Cognitive Computing
## An Introduction

*A first-semester textbook, written as Jupyter notebooks*

**Author:** Er. Rishabh Aryan  
**Licence:** MIT  
**Copyright © 2026 Er. Rishabh Aryan**

---

## Author

**Er. Rishabh Aryan**  
M.Tech (Artificial Intelligence and Data Science)  
Department of Computer Science and Engineering  
Indian Institute of Information Technology, Bhagalpur (Bihar), India

- Institutional email: [rishabh.250201011@iiitbh.ac.in](mailto:rishabh.250201011@iiitbh.ac.in)  
- Personal email: [rishabharyan887@gmail.com](mailto:rishabharyan887@gmail.com)  
- ORCID: [https://orcid.org/0009-0004-7595-9440](https://orcid.org/0009-0004-7595-9440)

Correspondence regarding this manuscript may be addressed to either address above.

---

## Preface

### Why this book exists

The brain is not a keyboard. A computer is not a cortex. Between those two facts lies an engineering problem that has been named, for half a century, a brain–computer interface, and a modelling problem that has been named, with less discipline, cognitive computing. This book exists so that a serious student can hold both problems in one mind without collapsing them into a slogan.

A **brain–computer interface (BCI)** measures activity of the central nervous system and converts it into an artificial output that a person can, in the typical case, perceive and use: a letter, a cursor, a prosthetic command, a pulse of stimulation, a change in a display. That sentence is narrower than the public story, and it is meant to be. The public story speaks of chips that read thoughts, of minds uploaded, of intelligence poured from a skull into silicon. Those sentences are not definitions. They are advertisements for a future that has not consented to arrive. An introductory textbook that repeats them has already failed its first examination.

What *has* arrived is more interesting, and harder. Scalp sensors support communication when residual movement is gone. Cortical recordings coupled to language models turn attempted speech into text at rates that would recently have been dismissed as theatre. Closed loops pair decoded intention with robotics and stimulation in rehabilitation. Wearable devices estimate workload and attention with an accuracy that is sometimes useful and often oversold. None of this is magic. All of it is a pipeline: tissue, metal, noise, features, a model, an action, and a person who learns the model while the model learns the person.

**Cognitive computing** enters that pipeline as a neighbour, not as an alias. In this book the phrase has a working meaning: the design of computational systems that estimate, emulate, or adapt to cognitive functions — attention, working memory, decision, learning — whether or not those systems touch a living brain. From that neighbour, BCI borrows priors (a language model over intended words), policies (slow the speller when inferred fatigue rises), and, at the margin, neuromorphic hardware as a low-power front-end. It does not borrow a soul. The student who writes “the BCI is a cognitive computer” has produced a slogan. The student who writes “a language model is a prior over intended words” has produced a sentence this book can use.

A still narrower phrase, **cognitive BCI**, denotes an interface whose *target variable* is itself a cognitive state rather than a motor or linguistic output. Attention, memory, and affect are distributed, mixed, and unstable across context. They are legitimate scientific objects. They are not the same object as a cursor velocity. Chapter 8 exists so that this distinction survives contact with enthusiasm.

### What this book is, and what it is not

The field does not need another encyclopaedia. Authoritative volumes already treat neural engineering, BCI principles, and neural interfaces at handbook depth. This text does not replace them. It imposes order on a first semester.

The book is **generic and introductory**. It is written for advanced undergraduates and first-year postgraduate students in computer science, artificial intelligence, electrical engineering, biomedical engineering, and cognitive science. A reader who has completed linear algebra, elementary probability, a first course in machine learning, and the willingness to run Python should be able to finish it. Chapter 0 restores the mathematics and the coarsest neuroscience that mixed classrooms do not share. After that, the voice is single and the vocabulary is fixed.

The book is **not** a catalogue of firms, a market report, or a popular history of implants. Company names appear only when a sentence would be dishonest without them. Market forecasts do not appear at all. Performance numbers that cannot survive a causal time split are treated as artefacts. Organoid computers and whole-brain digital twins, if mentioned, belong in open questions, not in the definition of the subject.

### How the argument is organised

The course has a spine.

Chapters 0 and 1 establish language. A recording is a mixture, not a transcript. An inner product is a spatial filter. Bayes’ rule is how a prior changes a decode. A BCI is classified by invasiveness, by direction of information, and by purpose; it is further named active, reactive, or passive. Adjacent technologies — gaze tracking, electromyography, classical sensory implants — may be more useful in a given life and still not be BCIs.

Chapters 2–4 complete the foundation: a first engineering model of the brain; the resolution–risk surface of recording and stimulation; the closed loop in which user and decoder co-adapt.

Chapters 5–7 are the technical core that can be implemented: paradigms that already work (sensorimotor rhythms, P300, evoked potentials, attempted speech); traces to features without ritual; learning systems for neural time series, including the reasons generic machine-learning hygiene is not enough.

Chapter 8 returns to cognitive computing with the vocabulary held fixed: theories as sources of features and policies; passive and neuroadaptive interfaces; neuromorphic hardware as implementation, not metaphysics.

Chapters 9–11 apply the loop to communication and motor substitution, to rehabilitation, and to consumer and workplace systems that share a name with clinical implants and almost nothing else.

Chapter 12 concerns evaluation, translation, and ethics. Those topics are not an afterword. A device that works in a demonstration and is abandoned after a trial is not a success with an asterisk. It is a failure of the loop that includes the institution around the patient. Consent under dependency, ownership of neural data, mental privacy, and equity of access are operational constraints on design.

Appendix L is a laboratory that uses public data only, so that a course does not depend on a headset budget.

### Pedagogical contracts

Every chapter is a Jupyter notebook. Prose, numbered definition, equation, figure, and computation occupy the same page. Cells are meant to be executed in order. Exercises close each chapter; solutions are withheld from the public notebooks if the text is used as a course.

A running example, **Amina**, is a composite person with amyotrophic lateral sclerosis, not a patient file. She exists so that a method which requires two hundred fatiguing trials before breakfast cannot be called finished. When the book asks whether a BCI is the correct communication device, the presence of a reliable finger twitch is allowed to matter.

Mathematics is kept where it earns its keep. Linear algebra and probability appear in Chapter 0 and are reused, not re-derived. Deep models appear after features, not instead of them. Foundation-style neural decoders are described as tools with a list of unsolved problems, not as a verdict on the field.

### Claims this book will not carry

| Sentence you may meet | Position of this book |
|---|---|
| The headset reads your thoughts. | It records a mixed field and decodes a task-defined pattern. |
| Non-invasive equals equivalent. | Risk is lower; information grain is not equivalent. |
| Invasive equals clinically ready. | Surgical feasibility is not home use, maintenance, or consent over years. |
| Accuracy of ninety-five percent. | On which split, which baseline, which user, which session? |
| Artificial intelligence has solved BCI. | Models improved decoding. They did not remove calibration, drift, or obligation. |
| Cognitive computing is BCI. | One is a modelling and systems programme. The other is an interface. |

If you have come here to be thrilled, you will be disappointed in the correct way. The thrill that lasts is narrower: a clean definition, a leakage-safe experiment, a user who can still refuse, and a machine that does one modest thing when a nervous system cannot. Learn to build that, and to refuse everything that merely resembles it. The rest of the literature will still be there when you are ready to be less introductory.

### How to use the notebooks

```bash
pip install -r requirements.txt
jupyter lab chapters/chapter_00_refreshers.ipynb
```

Read Chapter 0 before Chapter 1. Do not skip the leakage demonstration; later chapters assume you have seen why a shuffled window split is not an evaluation.

### Prerequisites

- Linear algebra (vectors, inner products, eigenvalues at the level of principal component analysis)
- Probability and a first course in statistics
- Introductory machine learning
- Python 3

### Status of the manuscript

| Chapter | Aim | Status |
|--------:|----------|--------|
| — | README.md (this preface) | Complete |
| Chapter 0 — Two short refreshers | A mathematical note. | Complete |
| Chapter 1 — What an interface is | Give students a stable vocabulary and a reason to care before any filter equation appears. | Complete |
| Chapter 2 — A first model of the brain | Supply only the biology an engineer must not get wrong. | Complete |
| Chapter 3 — Measuring and stimulating | Make the resolution–risk trade-off the organising idea of the chapter. | Complete |
| Chapter 4 — The BCI loop | This is the spine of the course. Every later chapter hangs off one box in this diagram. | Complete |
| Chapter 5 — Paradigms that already work | Teach four families well rather than twenty names badly. | Complete |
| Chapter 6 — From traces to features | Make preprocessing a principled stage, not a ritual. | Complete |
| Chapter 7 — Learning systems for neural data | Connect the student’s existing machine-learning course to neural time series. | Complete |
| Chapter 8 — Cognitive computing in this setting | Separate three ideas students routinely fuse. | Complete |
| Chapter 9 — Communication and motor substitution | Move from bit-rate to a usable day. | Complete |
| Chapter 10 — Rehabilitation and closed loops | Show BCI as a therapy component, not only as a substitute limb. | Complete |
| Chapter 11 — Beyond the clinic | Teach the consumer and workplace layer without glamour. | Complete |
| Chapter 12 — Evaluation, translation, and ethics | Give students a professional conscience and a translation map. | Complete |
| Appendix L — Laboratory (optional but recommended)| Four sessions: (L1) inspect public EEG and plot spectra; (L2) P300 offline pipeline; (L3) motor-imagery classification with a leakage-safe split; (L4) design document for a hypothetical study, including an ethics checklist. All work on public datasets so the course does not depend on purchasing headsets. | Complete |

---

## MIT Licence

Copyright © 2026 Er. Rishabh Aryan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the “Software”), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

This licence governs the notebooks, the figures they generate, and this preface.
Place a file named `LICENSE` at the repository root containing the same text
so that GitHub detects the licence automatically.

---

*End of front matter.*

## 🔗 Other repositories by Rishabh Aryan

| Repository | Description | Live |
|---|---|---|
| [100-days-of-python](https://github.com/Rishabh-bgp/100-days-of-python) | My original, offline, no-API-key solutions to all 100 projects of the 100 Days of Code Python bootcamp curriculum… | — |
| [Agentic-Engineering-Ebook](https://github.com/Rishabh-bgp/Agentic-Engineering-Ebook) | Agentic Engineering is a practical notebook-book on specifying, generating, verifying, and refining multi-tenant… | — |
| [beed-ml-study](https://github.com/Rishabh-bgp/beed-ml-study) | Provenance audit and leakage-aware benchmark of seizure-type classifiers on the Bangalore EEG Epilepsy Dataset — IIT… | — |
| [building-a-virtual-cell-in-python](https://github.com/Rishabh-bgp/building-a-virtual-cell-in-python) | A cell has a normal gene-activity pattern. Knock out one gene and that pattern changes. This project trains a small… | — |
| [Chronic-Kidney-Disease-Stage-Identification-in-HIV-Infected-Patients-Using-Supervised-ML](https://github.com/Rishabh-bgp/Chronic-Kidney-Disease-Stage-Identification-in-HIV-Infected-Patients-Using-Supervised-ML) | ML is transforming Chronic Kidney Disease (CKD) detection in HIV patients, catching early asymptomatic stages to… | — |
| [cobratate](https://github.com/Rishabh-bgp/cobratate) | Cobratate, an esoteric imperative programming language. Tate-flavored syntax, ordinary semantics, and a Python… | [open](https://rishabh-bgp.github.io/cobratate/) |
| [coda-synth](https://github.com/Rishabh-bgp/coda-synth) | CoDA-Synth: stylometric detection of LLM-rewritten dark-web documents with sparse TF-IDF + LinearSVC. Research lab,… | [open](https://shale-ember-delta-kite.grok.me/) |
| [IIT-ROPAR-GENAI-FOUNDATIONS](https://github.com/Rishabh-bgp/IIT-ROPAR-GENAI-FOUNDATIONS) | Free open-source Generative AI foundations ebooks (2026) covering Claude, Grok, Gemini, Cursor, OpenAI and more —… | — |
| [kbc-game](https://github.com/Rishabh-bgp/kbc-game) | Kaun Banega Crorepati (KBC) quiz game for the terminal in Python: 16-question prize ladder, safe levels and 4… | — |
| [knn-classifier](https://github.com/Rishabh-bgp/knn-classifier) | Simple K-Nearest Neighbors classifier on the classic Iris dataset using scikit-learn. Loads data, trains the model,… | — |
| [linear-regression-model-](https://github.com/Rishabh-bgp/linear-regression-model-) | Supervised linear regression on the scikit-learn diabetes dataset. A single feature (BMI) is used to predict… | — |
| [logistic-regression](https://github.com/Rishabh-bgp/logistic-regression) | This graduate capstone applies multi-class logistic regression to the Iris dataset. It includes EDA, stratified… | — |
| [logistics-website-capstone](https://github.com/Rishabh-bgp/logistics-website-capstone) | Logistics website capstone: Kargonaut Logistics, a premium freight site mixing claymorphism, glassmorphism and… | [open](https://rishabh-bgp.github.io/logistics-website-capstone/) |
| [lovelight-leap](https://github.com/Rishabh-bgp/lovelight-leap) | 💖 Lovelight Leap: a love-themed 2D platformer in vanilla JS canvas. 4 worlds, a boss you cheer up, original… | [open](https://rishabh-bgp.github.io/lovelight-leap/) |
| [machine-learning-part-1](https://github.com/Rishabh-bgp/machine-learning-part-1) | Machine learning in Python with scikit-learn: heart disease classification and medical insurance cost regression… | — |
| [Meeting-of-Machines-Consumer-Agents-Seller-Agents-and-Hidden-Fulfilment-Risk-in-Online-Retail](https://github.com/Rishabh-bgp/Meeting-of-Machines-Consumer-Agents-Seller-Agents-and-Hidden-Fulfilment-Risk-in-Online-Retail) | Agentic commerce lets shopping and seller agents place orders without showing operational truth. This IS case argues… | — |
| [morocco-city-aware-load-forecasting](https://github.com/Rishabh-bgp/morocco-city-aware-load-forecasting) | City-aware short-term load forecasting and peak detection on high-resolution Moroccan smart-meter data (5 zones).… | — |
| [NIELIT-DATA-SCIENCE](https://github.com/Rishabh-bgp/NIELIT-DATA-SCIENCE) | Hands-on NumPy, Pandas, and Matplotlib Jupyter notebooks for the NIELIT Data Science curriculum — practical,… | — |
| [NIELIT-MACHINE-LEARNING-PROJECTS](https://github.com/Rishabh-bgp/NIELIT-MACHINE-LEARNING-PROJECTS) | Nineteen end-to-end machine learning projects: classification, regression, clustering, and recommendation, with… | — |
| [NIELIT-PYTHON-](https://github.com/Rishabh-bgp/NIELIT-PYTHON-) | Open-source Python teaching notebooks: a language reference and five capstone programs, with detailed documentation.… | — |
| [pan-cancer-classification](https://github.com/Rishabh-bgp/pan-cancer-classification) | Leakage, equivalence, conformal reliability and data efficiency on the UCI TCGA Pan-Cancer RNA-Seq dataset — IIT… | — |
| [Predicting-Hot-Events-in-the-Early-Period-through-Bayesian-Model-for-Social-Networks](https://github.com/Rishabh-bgp/Predicting-Hot-Events-in-the-Early-Period-through-Bayesian-Model-for-Social-Networks) | This notebook details the implementation and evaluation of a Bayesian perspective Early stage Event Prediction… | — |
| [prediction-as-power](https://github.com/Rishabh-bgp/prediction-as-power) | Laboratory and working paper on prediction as power in European electricity markets. A DE-like hourly simulator… | — |
| [snakes-and-ladders](https://github.com/Rishabh-bgp/snakes-and-ladders) | 🐍🪜 Original Snakes & Ladders browser game: hand-drawn SVG snakes and ladders, 3D dice, 2-4 humans or bots, sound,… | [open](https://rishabh-bgp.github.io/snakes-and-ladders/) |
| [spam-scan](https://github.com/Rishabh-bgp/spam-scan) | Explainable spam, phishing & Indian-scam detector for SMS/email (English, Hindi, Hinglish): TF-IDF + Logistic… | [open](https://spam-scan.onrender.com) |
| [vedic-math-hybrid-kt](https://github.com/Rishabh-bgp/vedic-math-hybrid-kt) | Hybrid Vedic Math AI: rule-based sutras (Urdhva-Tiryagbhyam, Nikhilam, Yavadunam) plus RF classifier that cleans… | — |
| [wind-turbine-power-model](https://github.com/Rishabh-bgp/wind-turbine-power-model) | Single-turbine power curves + wind-farm simulation. Weibull wind stats, hourly NASA-style speed data, and… | — |
| [zoo-website-capstone](https://github.com/Rishabh-bgp/zoo-website-capstone) | Capstone project: a fictional zoo website built twice — a beginner-style simple version and a cinematic advanced… | [open](https://rishabh-bgp.github.io/zoo-website-capstone/) |
