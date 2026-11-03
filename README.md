# computational-theory
SHA-256 implemented step-by-step in Python and NumPy, following the FIPS 180-4 Secure Hash Standard directly — Computational Theory assessment, ATU.

## What's here

- `problems.ipynb` — everything lives here: the problems, my notes on how I'm
  approaching each one, and the code itself
- `data/` — nothing in here yet, will hold any datasets if I end up needing them
- `img/` — same, empty for now, for any diagrams or plots
- `AGENTS.md` — conventions for the repo, copied from the module notes
- `requirements.txt` — packages needed to run the notebook

## What's in the notebook

Each problem has markdown explaining what I did and why, with the code and tests underneath. The notebook follows the [Secure Hash Standard](https://csrc.nist.gov/pubs/fips/180-4/upd1/final).

- **Problem 0:** I created GitHub issues to track my progress.
- **Problem 1:** How I represent the data SHA-256 uses in Python (words, messages, blocks and the hash).
- **Problem 2:** The bitwise functions SHA-256 uses (Ch, Maj, Σ0, Σ1, σ0 and σ1).
- **Problem 3:** Generating the 64 round constants from the cube roots of the first 64 primes, and checking them against the standard.

## How to run it

You need Python 3 (I used 3.14). Open a terminal and clone the repository:

```
git clone https://github.com/MarkJohnBowman/computational-theory.git
cd computational-theory
```

Make a virtual environment and activate it:

```
python -m venv .venv
.venv\Scripts\activate         # Windows
source .venv/bin/activate      # macOS or Linux
```

Install the requirements and open the notebook:

```
pip install -r requirements.txt
jupyter notebook problems.ipynb
```

If you don't have Jupyter, run `pip install notebook` first. Then choose Restart Kernel and Run All Cells to run everything. It only takes a few seconds.

