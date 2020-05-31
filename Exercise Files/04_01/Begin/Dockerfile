FROM python:3.7.3-slim

LABEL maintainer="Jonathan Fernandes <theolympicsguy@gmail.com>"
LABEL description="Dev environment for machine learning and data science team \
                  with access to shared data in network drive."

WORKDIR /data

COPY . /data

RUN pip install jupyter python==3.7.3 pandas==0.24.2 seaborn==0.9.0

EXPOSE 8888

VOLUME /data

CMD ["jupyter","notebook","--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]
