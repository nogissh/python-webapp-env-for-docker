FROM python-webapp-env_python-webapp-base:latest

# Install inquired modules
COPY ./requirements.txt /workspace/
RUN /bin/bash -c "source ~/.bash_profile && \
                  pip install -r /workspace/requirements.txt"

# Set server configs
RUN echo "daemon off;" >> /etc/nginx/nginx.conf
COPY ./docker/nginx-app.conf /etc/nginx/sites-available/default
COPY ./docker/supervisor-app.conf /etc/supervisor/conf.d/
COPY ./docker /home/docker

# Copy project to image
COPY . /home/docker/app

# Expose port
EXPOSE 80
