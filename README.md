# Brain–Computer Interfaces and Cognitive Computing  
## An Introduction

*A textbook in Jupyter notebooks*

---

## Preface

The brain is not a keyboard. A computer is not a cortex. Between those two facts lies an engineering problem that has been named, for half a century, a brain–computer interface — and a modelling problem that has been named, with less discipline, cognitive computing. This book is written so that a serious student can hold both problems in one mind without confusing them.

A brain–computer interface measures activity of the central nervous system and turns that activity into an artificial output: a letter, a cursor, a pulse of stimulation, a change in a machine that the user can perceive. That sentence is narrower than the public story, and it is meant to be. The public story speaks of chips that read thoughts, of minds uploaded, of intelligence poured from a skull into silicon. Those sentences are not definitions. They are advertisements for a future that has not consented to arrive. An introductory textbook that repeats them has already failed its first examination.

What *has* arrived is more interesting, and harder. Scalp sensors and cortical arrays now support communication when movement and speech are gone. Decoders coupled to language models turn attempted articulation into text at rates that would have been dismissed as theatre a decade ago. Closed loops pair intention with robotics and stimulation in the service of rehabilitation. Wearable devices estimate workload and attention with an accuracy that is sometimes useful and often oversold. None of this is magic. All of it is a pipeline: tissue, metal, noise, features, a model, an action, a person who learns the model while the model learns the person.

Cognitive computing enters that pipeline as a neighbour, not as an alias. It is the design of systems that estimate or adapt to attention, memory, decision, and learning. It supplies priors, policies, and — when the hardware is neuromorphic — a possible low-power front-end. It does not make a decoder into a mind. The student who writes “the BCI is a cognitive computer” has produced a slogan. The student who writes “a language model is a prior over intended words” has produced a sentence this book can use.

The field does not need another encyclopaedia. Authoritative handbooks already exist, and this text does not pretend to replace them. What it does instead is impose order on a first semester. Every chapter is a Jupyter notebook so that prose, equation, figure, and computation occupy the same page. Claims are classified before they are admired. Evaluation is treated as part of the method, not as a courtesy at the end. Ethics is not an afterword. A device that works in a demonstration and is abandoned after a trial is not a success with an asterisk. It is a failure of the loop that includes the institution around the patient.

You are expected to arrive with linear algebra, elementary probability, a first course in machine learning, and the willingness to run code. Chapter 0 restores the minimum of mathematics and neuroscience that mixed classrooms do not share. After that, the book proceeds in a single voice. Company names appear only when a sentence would be dishonest without them. Market forecasts do not appear at all. Performance numbers that cannot survive a causal time split are treated as artefacts.

If you have come here to be thrilled, you will be disappointed in the correct way. The thrill that lasts is narrower: a clean definition, a leakage-safe experiment, a user who can still say no, and a machine that does one modest thing when a nervous system cannot. Learn to build that, and to refuse everything that merely resembles it. The rest of the literature will still be there when you are ready to be less introductory.

— *The author*

---

## How this book is organised

| Chapter | Notebook | Subject |
|--------:|----------|---------|
| 0 | `chapters/chapter_00_refreshers.ipynb` | Mathematical and neuroscience refreshers |
| 1 | `chapters/chapter_01_what_an_interface_is.ipynb` | Definition, history, taxonomies, neighbouring fields |
| 2 | *forthcoming* | A first model of the brain |
| 3 | *forthcoming* | Measuring and stimulating |
| 4 | *forthcoming* | The BCI loop |
| 5 | *forthcoming* | Paradigms that already work |
| 6 | *forthcoming* | From traces to features |
| 7 | *forthcoming* | Learning systems for neural data |
| 8 | *forthcoming* | Cognitive computing in this setting |
| 9 | *forthcoming* | Communication and motor substitution |
| 10 | *forthcoming* | Rehabilitation and closed loops |
| 11 | *forthcoming* | Beyond the clinic |
| 12 | *forthcoming* | Evaluation, translation, and ethics |
| L | *forthcoming* | Laboratory appendix |

## Running the notebooks

```bash
pip install -r requirements.txt
jupyter lab chapters/chapter_00_refreshers.ipynb
```

Execute each notebook from top to bottom. Chapter 0 is required before Chapter 1. Exercise solutions are withheld from the public notebooks.

## Prerequisites

- Linear algebra (vectors, inner products, eigenvalues at the level of PCA)
- Probability and a first statistics course
- Introductory machine learning
- Python 3

## Licence

Add the repository licence before public release.
