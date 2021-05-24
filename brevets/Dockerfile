FROM python:3.8
LABEL maintainer="jcsdavis@gmail.com"
COPY . /todo
WORKDIR /todo
RUN pip install -r requirements.txt
RUN chmod +x run_tests.sh
