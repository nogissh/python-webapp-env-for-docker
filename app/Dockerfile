FROM python-webapp-env_python-webapp-base:latest

# Install inquired modules
COPY ./requirements.txt /workspace/
RUN /bin/bash -c "source ~/.bash_profile && \
                  pip install -r /workspace/requirements.txt"
