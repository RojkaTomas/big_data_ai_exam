FROM python:3.12.0-alpine

WORKDIR /app

# Copy the application folder inside the container
COPY . . 

# Install the necessary dependencies
RUN apk add --no-cache gcc musl-dev postgresql-dev
RUN pip install -r requirements.txt

EXPOSE 8000

CMD ["python", "app.py"]
