FROM rocker/r2u:22.04

RUN apt-get update && apt-get install -y --no-install-recommends \
  git \
  python3 \
  python3-pip \
  && rm -rf /var/lib/apt/lists/*

RUN pip3 install radian

RUN install2.r --error --skipinstalled --ncpus -1 \
  languageserver \
  httpgd \
  conflicted \
  tidyverse

RUN installGithub.r MilesMcBain/breakerofchains lionel-/codegrip

CMD ["radian"]
