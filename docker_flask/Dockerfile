# Su dung image python:3.9-slim-buster
FROM python:3.9-slim-buster

# Thiet lap  working directory
WORKDIR /app

# Copy file requirements.txt
COPY requirements.txt .

# Cai dat cac thu vien can thiet
RUN pip install -r requirements.txt

# Mo port 5000
EXPOSE 5000

# Thiet lap bien moi truong
ENV FLASK_APP=hello_flask.py

# Copy code vao container
COPY . .

#Khoi chay app
CMD ["flask", "run", "--host", "0.0.0.0"]

