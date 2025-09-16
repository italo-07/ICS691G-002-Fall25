# Generative AI for Pull Request Descriptions: Adoption, Impact, and Developer Interventions

**Published in:** *Proceedings of the ACM on Software Engineering (PACMSE)*
**Authors:** Tao Xiao (Nara Institute of Science and Technology, Japan), Hideaki Hata (Shinshu University, Japan), Christoph Treude (Singapore Management University, Singapore), Kenichi Matsumoto (Nara Institute of Science and Technology, Japan)
**Link:** [ACM Digital Library](https://doi.org/10.1145/3643773)

The study examines GitHub’s Copilot for Pull Requests (PRs), a generative-AI service that auto-generates PR descriptions via marker tags such as *copilot\:summary* and *copilot\:walkthrough*. Analyzing 18,256 Copilot-generated PRs from 146 open-source repositories (and 54,188 non-Copilot PRs as a control), the authors employ mixed methods: quantitative quasi-experiments with propensity-score weighting and qualitative coding of 1,437 revisions where developers edited AI-suggested content.

Results show a steady rise in adoption, with the *copilot\:summary* tag appearing 13,231 times and the *copilot\:summary* + *copilot\:walkthrough* combination used in 5,598 PRs. PRs enhanced by Copilot require significantly less review time—an average reduction of 19.3 hours (ATT = -19.3 h)—and are 1.57 times more likely to be merged (OR = 1.57, p < 0.001).

Qualitative analysis uncovers 13 categories of supplementary information added by developers, the most frequent being static-template content (22.8%) and associated links (22.7%). Seven editorial actions modify AI output, dominated by partial deletions (22.9%) and refinements (20.8%). Developers also replace or augment AI-generated sections, illustrating a collaborative “human-AI” workflow.

The authors conclude that Copilot for PRs improves efficiency and merge success, while highlighting the need for better template integration and developer-specific suggestions to reduce unnecessary edits. They recommend broader adoption, embedding Copilot tags into PR templates, and refining the tool to tailor content to repository contexts. The work provides the first large-scale empirical evidence of generative-AI’s impact on the PR review process and informs future tool design.
