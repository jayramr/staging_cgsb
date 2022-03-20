Install BioSAILs Quick Start
============================

Basic Introduction
------------------

BioSAILs has been developed by a small Core Bioinformatics team that is focused on managing and analyzing substantial amounts of high throughput sequencing data. When designing BioSAILs, we needed to take account of the following,



Design a system that is agnostic as to the OS/Hardware combination it was running on (as long as it’s UNIX based).
Enable reproducible research.
Have a simple command line interface.
Flexible and easy to modify analysis workflows.
Can submit and track analysis workflows whether it’s on a high performance computing cluster, or a standalone Laptop.
Agnostic as to where bioinformatics software is installed.


BioSAILs has enabled us to analyze data from Metagenomics (shotgun/amplicon), RNAseq, Genome/Exome resequencing, de novo genome/transcriptome, epigenome (CHiPseq/ATACseq), and we believe it is now at a stage where the wider scientific community would benefit from using it. We hope to have a catalogue of community and in-house developed workflows that can be reused and adapted, without the need to write pipelines from scratch.



On this website, you will find :ref:`everything <settingup>` that we have put together in order to make it as easy as possible for you to start using BioSAILs. We also have a section dedicated to setting up a bioinformatics infrastructure.



If this is your first visit, we suggest you start with this guide here, which will take you from “No BioSAILs” all the way to reading an interesting paper and translating that into an analysis workflow.

.. figure:: /images/cgsb.png
   :alt: Biosails Workflow

   *Figure: Biosails Workflow Diagram*


Install on Linux
-----------------

.. code-block:: none

    wget https://repo.continuum.io/archive/Anaconda3-5.0.1-Linux-x86_64.sh
    bash Anaconda3-5.0.1-Linux-x86_64.sh
    conda install -c bioconda -c conda-forge perl-hpc-runner-command perl-biox-workflow-command

Install on MacOSX
------------------

.. code-block:: none

    wget https://repo.continuum.io/archive/Anaconda3-5.0.1-MacOSX-x86_64.sh
    bash Anaconda3-5.0.1-MacOSX-x86_64.sh
    conda install -c bioconda -c conda-forge perl-app-cpanminus
    cpanm HPC::Runner::Command BioX::Workflow::Command

