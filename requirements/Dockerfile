FROM python:3.9

COPY u2net.onnex /home/.u2net/u2net.onnex

WORKDIR /app

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 5100

CMD [ "python", "app.py" ]

