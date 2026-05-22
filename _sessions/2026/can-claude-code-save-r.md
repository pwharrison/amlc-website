---
layout: session-2026
title: "Can Claude Code Save R?"
permalink: /2026/sessions/can-claude-code-save-r/
youtube_id: WCK0JSuuZo8
---

# Can Claude Code Save R?

**Friday, April 17, 2026 · 11:30 AM – 12:00 PM · Violet Crown Charlottesville**

---

I use R every day for bioinformatics in 3 use cases: writing and maintaining R packages, routine bioinformatics analysis, and data exploration as part of research. Over the last 3 months, I have leaned heavily on Claude Code to help with these use cases.

The flip side of R’s richness and flexibility is its complexity: > 23,000 packages on CRAN, > 2,300 packages in Bioconductor, at least 4 (?) object oriented systems (S3, S4, Reference Classes, R6), 4 table-like types: matrices, data.frames, data.tables, and tibbles, and 3 packages for working with strings and regular expressions.

Agentic coding seems well suited to navigating these complexities. I propose that we can develop best practices and software (standard prompts, /skills, hooks/automated workflows) to make agentic coding in R more usable and reliable. 

For writing and maintaining R packages, Claude Code has worked well for me “out of the box”. It was notably useful for profiling code and then improving performance. In a similar vein, is it possible for Claude Code to check test coverage and suggest new tests? I also hypothesize that we can ask a coding agent to reliably ensure that the documentation agrees with the code beyond what R CMD check offers. Can it often infer return types and argument types in the context of the entire code base? Would it be beneficial for the coding agent to use type annotations for partial type checking? For code readability, should we ask the coding agent to consistently use tidyverse (but if performance dictates, use data.table operations and leave the tidy code as comments)?

Claude Code has also done well with common bioinformatics workflows such as “bulk” RNA-sequencing, single-cell RNA-sequencing. It ought to be possible to integrate this with codified workflows in repositories such as nf-core. 

Final analysis and presentation for publication seem more challenging. I still find that adjusting plots and plot layouts and organizing data using quarto tend to be time sinks. I hope that there is a way to help Claude Code understand ggplot2 better and develop quarto markdown that is better factored and supports faster iteration over design.

Given the newness and incredibly fast development of agentic coding, it would be great to find an organizational home for an “agentic coding for R” user group to compare notes and share experience.

## About the Speaker

<div class="speaker-profile">
    <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/Steve_Rozen.png" alt="Steve Rozen">
  </div>
  <div class="speaker-profile-info">
    <h3>Steve Rozen</h3>
    <p><em>Director of Bioinformatics and Research Computing, Duke University School of Medicine</em></p>
    <p>Steve Rozen's research has spanned bioinformatics, human genetics, and cancer “multi-omics”. 

His work on bioinformatics and cancer was part of collaborations that led to multiple papers. This research was recognized by the American Association for Cancer Research 2018 Team Science Award for work on aristolochic acid mutagenesis in liver and urinary tract cancers and for studies of biliary tract cancers, lymphomas, and gastric cancers. 

Within genomics, he has recently studied mutational signatures as tools for discovering the causes of mutations in cancer and for studying mechanisms of DNA damage and repair. His reference paper on mutational signatures has been cited > 3000 times since 2020. 

Previously, Rozen also created and maintained the widely-used Primer3 software for PCR primer design and worked extensively on identifying mutations in the human Y chromosome and their clinical consequences.</p>
  </div>
</div>
