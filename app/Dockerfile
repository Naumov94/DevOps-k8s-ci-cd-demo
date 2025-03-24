# 1. Use official Python image
FROM python:3.10-slim

# 2. Set working directory inside container
WORKDIR /app

# 3. Copy dependencies and install them
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# 4. Copy application code
COPY app.py .

# 5. Run the Flask application
CMD ["python", "app.py"]
