
# Use the same Python version family as the backend
FROM python:3.13-slim

# Set the application folder
WORKDIR /app

# Copy the frontend files
COPY . .

# Install dependencies
RUN pip install --no-cache-dir --upgrade pip
RUN pip install --no-cache-dir -r requirements.txt

# Start the frontend on port 8501
CMD ["streamlit", "run", "app.py", "--server.port=8501", "--server.address=0.0.0.0"]
