FROM python:3.10-slim

WORKDIR /app

COPY app.py /app/
COPY spam_classifier_model.pkl /app/
COPY tfidf_vectorizer.pkl /app/
COPY templates /app/templates

RUN pip install --no-cache-dir flask scikit-learn joblib

EXPOSE 5000

CMD ["python", "app.py"]

