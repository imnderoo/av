# Base Image
FROM biocontainers/biocontainers:latest

# Metadata
LABEL base.image="biocontainers:latest"
LABEL software="AnnoVar"
LABEL software.version="20150617"
LABEL website="http://annovar.openbioinformatics.org/en/latest/"
LABEL documentation="http://annovar.openbioinformatics.org/en/latest/"
LABEL license="http://annovar.openbioinformatics.org/en/latest/"
LABEL tags="Genomics"

# Maintainer
MAINTAINER Andrew Wong <nderoo.wong@gmail.com>

# R dependencies

USER root

COPY . /tmp/

RUN unzip /tmp/package.zip && \
	cp *.pl /usr/bin/

CMD ["table_annovar.pl"]
