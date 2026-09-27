# Resources

A collection of tools, papers, and workflows I've found useful.

## Papers

- [Classic population genetics papers](https://morrelllab.github.io/classics/index.html) — curated by the Morrell Lab
- Pollak, Edward. "On the theory of partially inbreeding finite populations. I. Partial selfing." *Genetics* 117.2 (1987): 353.

## Tools & Workflows

### Custom ollama models

The below workflow creates a coding agent whose goal is to help guide graduate students. 

```
vim Modelfile
ollama create chip-assist -f ./Modelfile
ollama cp chip-assist milesdroberts/chip-assist
ollama push milesdroberts/chip-assist
```

This is the Modelfile

```
# 1. Choose your base model (e.g., llama3.2, gemma2, mistral, etc.)
FROM qwen3.8

# 2. Adjust parameters (Optional)
# Temperature: Higher means more creative/random, lower means more coherent
PARAMETER temperature 0.7
# Context window: Size of the model's memory in tokens
PARAMETER num_ctx 200000

# 3. Set the core personality or system prompt
SYSTEM """

Your name is Chip.

You are an AI research companion for a graduate student. Your job is not to
produce the fastest path to a finished analysis, figure, or paragraph — it
is to help the student build the judgment, technical skill, and research
instincts they'll need to do independent work, defend their choices to an
advisor or committee, and stand behind anything that eventually gets
published. You should be genuinely and substantially helpful — this is real
research, not an exercise — but you should be alert to moments where the
*way* they're using you would leave them unable to explain, reproduce, or
defend their own work, and say so directly.
"""
```

### RAG CLI

A simple CLI tool for asking questions about papers using retrieval augmented generation.

<https://github.com/milesroberts-123/custom-rag-cli/tree/main>

### Containerizing Snakemake workflows

Generate a Dockerfile from a Snakemake workflow with `snakemake --containerize > Dockerfile`.

<https://github.com/snakemake/snakemake/issues/2602>

### Snakemake + R Markdown

Embed an R Markdown notebook as a Snakemake rule to generate reports.

<https://nbis-reproducible-research.readthedocs.io/en/course_2104/rmarkdown/#r-markdown-and-snakemake>

