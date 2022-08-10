FROM postgis/postgis:14-3.2

RUN apt-get -qq update --yes \
  && apt-get -qq install --yes --no-install-recommends \
  build-essential ca-certificates \
  postgresql-plpython3-14 \
  && rm -rf /var/lib/apt/lists/*

ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update -y \
    && apt-get install -y \
      postgresql-14-plr \
      postgresql-14-postgis-3-scripts \
      postgresql-plpython3-14 \
      postgresql-contrib \
    && rm -rf /var/lib/apt/lists/*
