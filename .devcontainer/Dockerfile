FROM rocker/r2u:22.04

RUN apt-get update && apt-get install -y --no-install-recommends \
    git \
    python3 \
    python3-pip \
    && rm -rf /var/lib/apt/lists/*

RUN pip3 install --disable-pip-version-check \
    radian

RUN install2.r --error --skipinstalled --ncpus -1 \
    clipr \
    conflicted \
    dotenv \
    httpgd \
    janitor \
    languageserver \
    R6 \
    reprex \
    shiny \
    skimr \
    styler \
    tidyverse

RUN installGithub.r \
    cynkra/constructive \
    dreamRs/prefixer \
    lionel-/codegrip \
    ManuelHentschel/vscDebugger \
    MilesMcBain/breakerofchains \
    MilesMcBain/datapasta

CMD ["radian"]
