FROM python:3
RUN mkdir -p /home/app
COPY . /home/app
WORKDIR /home/app
RUN pip install -r requirements.txt && python -m textblob.download_corpora
EXPOSE 5000
CMD ["python3" "sentiment_analysis.py"]