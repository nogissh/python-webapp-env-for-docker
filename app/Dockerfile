FROM python-webapp-env:latest

# Install inquired modules
COPY ./requirement.txt /workspace
RUN /bin/bash -c "source ~/.bash_profile && \
                  pip install -r /workspace/requirement.txt"
