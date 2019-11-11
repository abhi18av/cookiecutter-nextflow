FROM nfcore/base
LABEL authors="author-name" \
      description="Docker image containing all requirements for the pipeline"

COPY environment.yml /
RUN conda env create -f /environment.yml && conda clean -a
ENV PATH /opt/conda/envs/nf-core-mnaseseq-1.0dev/bin:$PATH
