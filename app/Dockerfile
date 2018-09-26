FROM python-webapp-env:latest

# Install inquired modules
COPY ./requirements.txt /workspace/
RUN /bin/bash -c "source ~/.bash_profile && \
                  pip install -r /workspace/requirements.txt"
