# ARTIC SARS-CoV-2 Workflow

This repository contains a [nextflow](https://www.nextflow.io/) workflow for
running the ARTIC SARS-CoV-2 workflow on multiplexed MinION, GridION, and
PromethION runs.

## Quickstart

The workflow uses [nextflow](https://www.nextflow.io/) to manage compute and 
software resources, as such nextflow will need to be installed before attempting
to run the workflow.

The workflow can currently be run using either
[Docker](https://www.docker.com/products/docker-desktop) or
[conda](https://docs.conda.io/en/latest/miniconda.html) to provide isolation of
the required software. Both methods are automated out-of-the-box provided
either docker of conda is installed.

It is not required to clone or download the git repository in order to run the workflow.
For more information on running EPI2ME Labs workflows [visit out website](https://labs.epi2me.io/wfindex).

**Workflow options**

To obtain the workflow, having installed `nextflow`, users can run:

```
nextflow run epi2me-labs/wf-artic --help
```

to see the options for the workflow.

**Workflow outputs**

The primary outputs of the workflow include:

* a [FASTA](https://en.wikipedia.org/wiki/FASTA) file containing the consensus sequence for all samples,
* a [VCF](https://en.wikipedia.org/wiki/Variant_Call_Format) file sample all samples,
* an HTML report document detailing QC metrics and the primary findings of the workflow.


## Useful links

* [medaka](https://www.github.com/nanoporetech/medaka)
* [artic](https://github.com/artic-network/fieldbioinformatics)
* [nextflow](https://www.nextflow.io/)
* [docker](https://www.docker.com/products/docker-desktop)
* [conda](https://docs.conda.io/en/latest/miniconda.html)
