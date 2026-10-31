# Definite Extensions: Technical Supplement

Technical companion to *Definite Extensions: Rigidity, Circumscription, and Critical Plural Logic*, revised 31 October 2026.

- [Read the technical supplement (PDF)](definite-extensions-supplement.pdf)
- [LaTeX source](definite-extensions-supplement.tex)

The main paper states the results and their assumptions. This supplement provides the calculus, proofs, model constructions, and countermodels, with a notation guide. Main-text sections and equation numbers are distinguished from the supplement's lettered numbering.

| Main paper | Results | Supplement |
| --- | --- | --- |
| Section 3 | Quantifier characterization; comparison under the modal basis assumption; insufficiency of normal S4 alone | A.2; B.1–B.2 |
| Section 4 | Extensional representation; identity collapse; separation and nonpersistence of extensional definiteness | A.2; B.3; F.3 |
| Section 5 | Elementary closure, definite separation, Boolean operations, uniform union, and nonderivability of stronger closure principles | C; F.1 |
| Section 6 | Classification, critical principles without a universal plurality, and independence of Infinity | D.3–D.6 |
| Section 7 | Derived set axioms and joint consistency relative to ZFC | E |
| Section 8 | Constant-domain and S5 obstructions | F.2 |

The combined set-theoretic consistency model takes the definiteness operator to be broad necessity. It does not establish essential membership or joint consistency of all set axioms with distinct modalities. These qualifications are retained in both documents.

## Build

The source is self-contained and uses standard LaTeX packages. Run twice:

```sh
pdflatex definite-extensions-supplement.tex
pdflatex definite-extensions-supplement.tex
```

Cross-document reference numbers are synchronized with the 31 October 2026 main paper. For a fixed citation, use GitHub's permalink to the relevant commit rather than a moving branch URL.

## Provenance

AI-generated research draft developed from Andrew Bacon's proposal and preliminary model, then revised in response to his annotations. The supplement includes a fuller acknowledgment.
