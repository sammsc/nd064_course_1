FROM python:3.8
RUN mkdir /app
COPY techtrends /app/
WORKDIR /app
RUN pip install -r requirements.txt
EXPOSE 3111
RUN python init_db.py
CMD [ "python", "app.py" ]