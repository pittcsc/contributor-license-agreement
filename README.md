# PittCSC CLA

Welcome to the central repository for the Contributor License Agreement (CLA) of PittCSC! This repository hosts the agreement that contributors must acknowledge when contributing to CSC infrastructure, and the automated bot that manages signatures across all projects. 

## Why do we require a CLA?

Students across the world rely on CSC maintained tools and infrastructure, whether it's a someone at Pitt trying to figure out their classes, somebody else trying to apply to Steelhacks, or somebody who's using the simplify repo to apply to jobs. It is imperative we have an agreement that ensures contributors own their work since it has the potential to impact any number of people.

Read the full agreement here: [CLA Document](https://github.com/pittcsc/contributor-license-agreement/blob/main/CLA.md).

## How to Sign

You do not need to print or email any documents.
We use an automated bot to handle signatures directly within GitHub.

When you submit your first Pull Request to any repository under the PittCSC organization, simply leave the following exact phrase as a comment on your PR:

> I have read and agree to the PittCSC CLA

### What happens next?

1. Our centralized GitHub Action will detect your comment.
2. The bot will securely record your GitHub Handle, ID, and the timestamp in our public [`signatures/cla.json` registry](https://github.com/pittcsc/contributor-license-agreement/blob/main/signatures/cla.json).
3. The bot will leave a confirmation comment on your PR indicating that your signature was successful.

You only need to sign the agreement once. After your signature is recorded, you are cleared to contribute to any repository within the organization.

## Note for Maintainers

Any new repository made must include the [cla-sign-listener.yml](https://github.com/pittcsc/contributor-license-agreement/blob/main/.github/workflows/cla-sign-listener.yml) and [cla-verify-listener.yml](https://github.com/pittcsc/contributor-license-agreement/blob/main/.github/workflows/cla-verify-listener.yml) in `.github/workflows/`, and the Personal Access Token (PAT) must be added to the Repository Secrets under `CLA_BOT_PAT` with the following fine-grained permissions:

- Read access to metadata
- Read and write access to code and pull requests

Or you can create a new repository using our premade template, and all that needs to be done is adding the PAT. 

## AI-Generated Code and Intellectual Property

PittCSC values first-principles engineering and true concept mastery. Because of that, we encourage our software contributions to reflect genuine human authorship. After all, this is a school club, so to promote an enviornment of learning and to reduce pressure on contributors across all backgrounds, we have this agreement between the club and the contributor to not submit code generated purely by Artificial Intelligence (AI).

### There are many reasons to encourage students to follow this agreement

We know that large language models (LLMs) can write functional code. This allows for people to accomplish feats that they may not be capable of otherwise, and can increase productivity across the board. However, there is just as great of a negative effect, and we want you to understand is what the evidence actually says about what that costs you, and why this agreement exists.

### The Current Research on Cognitive Debt

There are many examples of research about how LLMs and their effects on people.

1) A [2025 randomized controlled trial](https://www.pnas.org/doi/10.1073/pnas.2422633122) with nearly 1,000 students found that students given unrestricted access to GPT-4 performed 48% better during practice, but 17% worse on exams when the tool was taken away. They had learned less than students who had no AI at all. Worst of all, they did not realize they were learning less, as they rated their own learning just as highly as the control group.
2) An [MIT Media Lab study](https://arxiv.org/abs/2506.08872) tracked brain activity over four months and found that LLM users showed progressively weaker neural engagement. When the LLM was removed, their cognitive activity did not bounce back. The researchers describe this as “cognitive debt”: short-term convenience purchased at the cost of deeper encoding.
3) A [Gallup/Walton Foundation survey](https://hbr.org/2026/01/how-gen-z-uses-gen-ai-and-why-it-worries-them) of 2,500 adults in their early twenties found that 79% believe AI makes people lazier and 62% worry it makes people less intelligent, yet 74% used it in the past month anyway. One in six reported using it at work even when told not to. People are not unaware of the problem, they're stuck in it. 

### Industry Trends Since ChatGPT Launched

A [Stanford Digital Economy Lab study](https://digitaleconomy.stanford.edu/publication/canaries-in-the-coal-mine-six-facts-about-the-recent-employment-effects-of-artificial-intelligence/) tracking millions of U.S. workers through ADP payroll data found that employment for software developers aged 22–25 has declined nearly 20% from its late-2022 peak, while employment for developers aged 35–49 has grown.

Entry-level hiring at major tech companies dropped roughly 25% year-over-year in 2024. In an [industry survey](https://www.cutimes.com/2024/05/14/8-in-10-hiring-managers-say-recent-grads-will-get-laid-off-due-to-ai-413-203360/) of 800 hiring managers, 70% said they believe AI can do the work of interns. The junior roles that used to be the on-ramp to a career are disappearing.

### What does this mean?

This means that the world is changing, and that the people getting hired are the ones who can do things LLMs cannot, and can be better, faster, and equally reliable when using an LLM. Now more than ever, it's important to build skills in understanding system failures, debugging problems you haven't encountered before, designing core data structures and architectural designs for projects, and explaining your reasoning to other people. This isn't something you build by reading an LLMs output, but by struggling through problems yourself, getting stuck, fixing the problem, getting stuck again, and then finally getting it right. 

We hope that the projects at CSC can exist as opportunities for people to be challenged, and to provide the enviornments and support for you to overcome those challenges and problems. 


### Permitted and Prohibited Uses of AI

We recognize that modern development across the industry does include AI-assisted development, and we want to clarify that there is a difference between tooling and authorship. The first time you do something, you should do it yourself. The fifth, tenth, fifteenth time, AI can increase your productivity because you have the _mental model_ to evaluate whether its output is correct. You cannot evaluate what you do not understand, and you cannot understand what you have never struggled through.

Using AI tools (e.g., GitHub Copilot, Tabnine, or ChatGPT) as a highly advanced autocomplete, for generating standard boilerplate, finding syntax errors, or writing basic unit test scaffolding is permitted and does not require disclosure. The core logic, architectural decisions, and vast majority of the keystrokes must be yours.

However, Prompting an AI to write functions, classes, or modules and copy-pasting the raw output into our codebase does require disclosure, and it's then up to a maintainer to review the submitted code. A general rule of thumb we suggest is that if a court would consider the AI as the primary author of a specific block of code, it cannot be merged into any repository.


## Attribution and Acknowledgements

PittCSC is grateful to the open source communities that inspire us and many others. We'd like to thank the other examples of a CLA that inspired this one. 

- [Modular](https://github.com/modular)
- [Scientific Computing Studio](https://github.com/scienting)
- [PNAS](https://www.pnas.org)
- [MIT Media Lab](https://www.media.mit.edu)
- [Harvard Business Review](https://hbr.org)
- [Stanford Digital Economy Lab](https://digitaleconomy.stanford.edu)
- [Credit Union Times](https://www.cutimes.com)