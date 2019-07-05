# https://github.com/elastic/elasticsearch-docker
FROM docker.elastic.co/elasticsearch/elasticsearch:7.2.0

# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
USER root
RUN usermod -u 1100 elasticsearch
USER elasticsearch
RUN elasticsearch-plugin install https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v7.2.0/elasticsearch-analysis-ik-7.2.0.zip