# Resources

This is a repository of fun things I learn, but have no where to write them.

## Favorite papers list

https://morrelllab.github.io/classics/index.html

### Population genetics

Pollak, Edward. "On the theory of partially inbreeding finite populations. I. Partial selfing." Genetics 117.2 (1987): 353.

## Building an AI agent to ask questions about papers on a SLURM cluster?

I made a simple CLI python script to pull papers and use a LLM to answer questions about the papers with retrival augmented generation.

https://github.com/milesroberts-123/custom-rag-cli/tree/main

## Containerizing snakemake workflows

https://github.com/snakemake/snakemake/issues/2602

Create docker file with `snakemake --containerize > Dockerfile`. Copy Dockerfile and envs to same directory. Then run these commands from a computer with docker:

```sh
sudo docker build -t poolseq-kmers .
sudo docker login -u milesroberts
sudo docker tag poolseq-kmers milesroberts/poolseq-kmers
sudo docker push milesroberts/poolseq-kmers
```

## Snakemake reports from rmarkdown

Could be a good idea to move my notebook into scripts, which will generate figures that get compiled into a snakemake report. In my mind, this is more easily reproducibile than having someone configure a notebook. However, you can't really explore the data this way beyond whatever figures you predetermine.

Another option is to just add my notebook as a snakemake rule:

https://nbis-reproducible-research.readthedocs.io/en/course_2104/rmarkdown/#r-markdown-and-snakemake

This could be nicer because R markdown will give me more control over what the report.html looks like.

