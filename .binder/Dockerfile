FROM rocker/binder:4.4.2
LABEL maintainer='Rhian Davies'
COPY --chown=${NB_USER} . ${HOME}
USER ${NB_USER}



RUN wget https://github.com/StatsRhian/Demo-quarto-for-managers/raw/master/DESCRIPTION && R -e "options(repos = list(CRAN = 'http://mran.revolutionanalytics.com/snapshot/2025-02-01/')); devtools::install_deps()"

RUN rm DESCRIPTION.1; exit 0
