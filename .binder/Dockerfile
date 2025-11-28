FROM rocker/binder:4.5.2
LABEL maintainer='Rhian Davies'
COPY --chown=${NB_USER} . ${HOME}
USER ${NB_USER}



RUN wget https://github.com/StatsRhian/demo-quarto-for-managers/raw/main/DESCRIPTION && R -e "options(repos = list(CRAN = 'http://mran.revolutionanalytics.com/snapshot/2025-11-28/')); devtools::install_deps()"

RUN rm DESCRIPTION.1; exit 0
