# AI Interview Questions and Answers

Code companion to *Artificial Intelligence Interview Questions and Answers* — a book of 284 questions covering what people actually get asked at AI and data science interviews.

This repo holds the runnable code from the book, plus a few things the book couldn't include: tests that prove the snippets work, a setup that won't fight you, and notebooks for the chapters where watching values change over time matters more than reading about it.

## A word before you dive in

The book started as a list of links I kept sending to friends preparing for interviews. After the fifth or sixth time pasting the same five GitHub repos and three textbook chapters into a chat, I decided to just write the thing. Three years later, here we are.

The code in this repo isn't meant to be production-grade. It's meant to be readable. If you want the fastest possible gradient descent, use PyTorch. If you want to understand what PyTorch is doing under the hood — and convince an interviewer you understand it — read what's here.

## What's in here

The book has 12 parts; the repo mirrors them, but only for chapters where the code adds something. Plenty of questions are conceptual and don't need a `.py` file attached.

```
ai-interview-questions/
├── code/
│   ├── search/             # BFS, DFS, IDDFS, UCS, A*
│   ├── ml/                 # Gradient descent, target encoding, bootstrap CIs
│   ├── deep_learning/      # Backprop from scratch, MAML inner loop
│   ├── computer_vision/    # Transfer learning, IoU, NMS
│   ├── nlp/                # BPE tokenizer, attention from scratch
│   ├── reinforcement/      # Q-learning, REINFORCE, MCTS sketch
│   ├── mlops/              # Pipeline pattern, A/B test analysis
│   └── time_series/        # Feature engineering, rolling anomaly
├── sql/                    # The queries from the SQL chapter
├── notebooks/              # When inline plots help more than prose
├── tests/                  # pytest, small but real
├── book/                   # LaTeX source — bring your own bibliography style
└── docs/                   # Errata, setup notes, references
```

## Getting set up

Python 3.10 or newer. The library pins aren't strict but I've only tested on the versions in `requirements.txt`.

```bash
git clone https://github.com/moussadoumbia/ai-interview-questions.git
cd ai-interview-questions
python -m venv .venv
source .venv/bin/activate          # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Confirm everything works:

```bash
pytest
```

If a test fails on your machine and not mine, please file an issue. That's almost always a real bug rather than a setup quirk, and I'd rather hear about it.

## How to use this repo

A few patterns I'd suggest depending on how you learn:

**Reading along with the book.** Each chapter directory has a small `README.md` that maps question numbers to files. So `code/search/README.md` tells you that question 3.6 (IDDFS) is in `iddfs.py`, and so on.

**Learning by running.** Every file in `code/` runs standalone. From the repo root:

```bash
python -m code.search.astar
python -m code.ml.gradient_descent
python -m code.deep_learning.backprop_scratch
```

Each one prints something useful — a solved puzzle, a loss curve, the recovered weights.

**Learning by breaking.** The files are short on purpose. Most are under 100 lines. They're meant to be edited until they break, then fixed. Fork the repo, change the activation function in `backprop_scratch.py` to ReLU, see what happens to convergence. That's the actual value.

**Notebooks.** For chapters where the point is to watch something evolve over training (loss curves, attention patterns, gradient norms, embedding drift), there's a notebook in `notebooks/`. Skip them if you prefer text; use them if you don't.

## What this repo is not

The README market is full of "comprehensive frameworks" and "production-ready implementations," so a few honest disclaimers:

- **Not a course.** That's the book. This repo is the appendix.
- **Not a framework.** Don't import from `code/` into your real ML pipelines. The implementations skip caching, error handling, and edge cases on purpose.
- **Not exhaustive.** Of 284 questions, maybe 60 have code here. The rest are conceptual or covered better by existing libraries.
- **Not a benchmark suite.** The examples are tiny by design. Toy datasets, small networks, short training runs.

## A note on the code style

You'll notice the code is heavier on comments than typical research code and lighter on abstraction than typical production code. That's intentional. When I read someone else's implementation, I want to know *why* a line is there, not just what it does. So I've over-commented in places where the reasoning isn't obvious from the code itself.

If you find a comment that's wrong, redundant, or condescending — open an issue. Bad comments are worse than no comments.

## Contributing

I'd love contributions, especially:

- Bug fixes and typo corrections.
- Clearer explanations or comments.
- Additional test cases.
- Implementations of the questions that don't currently have code.

What I'm less interested in:

- Rewriting things in a "more idiomatic" style for the sake of it.
- Adding heavy abstractions or frameworks.
- Optimizing for speed at the cost of readability.

See `CONTRIBUTING.md` for the workflow. The bar is whether the change makes the next reader's experience better.

The book text itself isn't open to contributions — that goes through separate editorial review — but errata reported here will get folded into future printings with credit.

## Citation

If the book or repo is useful to you, a citation is appreciated but not required:

```bibtex
@book{doumbia2026ai,
  title     = {Artificial Intelligence Interview Questions and Answers},
  author    = {Doumbia, Moussa},
  year      = {2026},
  publisher = {Self-published},
  url       = {https://github.com/moussadoumbia/ai-interview-questions}
}
```

## License

Code: MIT (see `LICENSE`). Use it however you like.

Book text and figures: copyrighted, not redistributable. Please don't paste the answers into commercial training material or competitor books without asking first. If you want to use a short passage for a blog post or review, that's fine — drop me a note so I know where it ended up.

## Contact

Errata, questions, or just want to say hi: open an issue, or email me at the address on my Howard University faculty page.

Good luck with the interview. The book is just a checkpoint — the real prize is leaving each prep session knowing a little more than you did when you started.

— Moussa
