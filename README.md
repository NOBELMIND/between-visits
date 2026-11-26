# Between Visits

*A case series from NOBELMIND. Where doctors get to feel like coders, and coders get to think like doctors.*

> **Invented patients only. Not medical advice.**
> Every patient here is fiction written for teaching. Please do not post real patient information anywhere in this repository, even de-identified. Edits stay visible in history, so a deleted detail is not truly gone.

## Why we do this

Most of a patient's care happens between visits. A patient goes home, steps on a scale each morning, writes down how they feel, and a clinician somewhere reads the log and decides whether today is the day to call. The hard part is rarely the textbook. It is noticing the quiet pattern in a page of ordinary numbers.

We wanted a place to practice that together. So we write invented patients, post their two weeks at home, and ask one question. Two weeks later we release the answer we wrote before the case went up, and talk about what we all saw and missed.

What we hope for:

- **Doctors** get a short, honest case to think about, and a gentle first taste of working on GitHub.
- **Developers** get to see how a clinician reads a home log, and why the obvious number is not always the important one.
- **Everyone** gets a conversation. The best part of a case is the discussion, not the reveal.

Physicians and engineers bring their specialization and ingenuity to build software that will expand the reach of medicine for everyone. We take this one case at a time, and corrections are welcome and credited.

## How to take part

1. Open the current case (see the case log below) and read it in your browser.
2. Decide what you would do. Write it down before you read anyone else's answer.
3. Share your answer one of two ways:
   - Open **Discussions**, find the case thread, and reply. Put your reasoning inside a collapsed block so you don't spoil it for others (the thread shows you how).
   - Or click **Issues → New issue → Answer a case** and fill in the short form.
4. Come back midway. The cardiologist may add a clue.
5. Two weeks after the case goes up, the answer is released. Compare, argue kindly, learn.

You need a free GitHub account to post. If you would rather not make one, send your answer to the person who invited you; we will only credit you by name if you say yes.

## Bring your own model

Point your favorite AI model at this repository and see what you can make from a case: a chart of the two weeks, a patient-friendly summary, a quiz, a second opinion to argue with. Then tell us in **Discussions** what you tried, what surprised you and where the model got it wrong.

- Share what you made as a link or a short write-up. Don't run other people's code unless you trust it.
- Use only the invented cases. Never give a model real patient information because of this project.
- Anything a model says about a case is for discussion, not medical advice.

## The sealed answer

Every answer is written by a cardiologist **before** the case is published. To show we did not change it after seeing your replies, we seal it:

1. The answer file and a long random "salt" file are kept private.
2. We publish only a fingerprint: the SHA-256 hash of the salt followed by the answer. It sits in `seal.txt` in the case folder, and the same fingerprint goes into a GitHub release on the day the case goes up.
3. On reveal day we publish the answer and the salt.

**Check it yourself** (Mac or Linux terminal, inside the case folder):

```
cat salt-01.txt answer-01.md | shasum -a 256
```

On Linux you can use `sha256sum` instead of `shasum -a 256`. If the result matches `seal.txt` and the release, the answer is the one we wrote before the case went up. Not a terminal person? Ask in the case discussion and a developer will walk through it with you.

What the seal shows: the answer did not change. What it does not show: that the answer is right. That part is for the discussion. If we get something wrong, we add a dated correction and never quietly rewrite a released answer.

## Momentum

This is where we keep score of the work, not the applause. Each case gets a release, so the list of releases is our changelog.

| Case | Title | Status | Answer |
|---|---|---|---|
| 1 | [His weight is perfect](cases/01-his-weight-is-perfect/) | Open | Sealed |

## Credit

Doctors and developers who add a clue, catch a mistake, suggest a case, or improve a page are named here (only with your permission).

| Name | What they added | Case |
|---|---|---|
| *Your name could be first* | | |

## Join in

- Read [CONTRIBUTING.md](.github/CONTRIBUTING.md) for a first contribution you can make entirely in your browser.
- Read the [Code of Conduct](.github/CODE_OF_CONDUCT.md). It is short.
- Licensing: terms are being finalized. Until then, all rights are reserved; you are welcome to read, discuss and take part here.

*Between Visits is run by NOBELMIND. Invented patients only. Not medical advice.*
