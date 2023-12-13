ARG buildtype
FROM python:${buildtype}
WORKDIR /app
ENV FLASK_APP=app.py
ENV FLASK_RUN_HOST=0.0.0.0
RUN apk add --no-cache gcc musl-dev linux-headers
COPY app.py /app
COPY requirement.txt /app
COPY .  .
RUN pip3 install -r requirement.txt
CMD [ "flask", "run" ]
