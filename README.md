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

| Chapter | Notebook | Status |
|--------:|----------|--------|
| — | `README.md` (this preface) | Complete |
| Chapter 0 — Two short refreshers | `A mathematical note.` | Complete |
| Chapter 1 — What an interface is | `Give students a stable vocabulary and a reason to care before any filter equation appears.` | Complete |
| 2 | A first model of the brain | In preparation |
| 3 | Measuring and stimulating | In preparation |
| 4 | The BCI loop | In preparation |
| 5 | Paradigms that already work | In preparation |
| 6 | From traces to features | In preparation |
| 7 | Learning systems for neural data | In preparation |
| 8 | Cognitive computing in this setting | In preparation |
| 9 | Communication and motor substitution | In preparation |
| 10 | Rehabilitation and closed loops | In preparation |
| 11 | Beyond the clinic | In preparation |
| 12 | Evaluation, translation, and ethics | In preparation |
| L | Laboratory appendix | In preparation |

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
