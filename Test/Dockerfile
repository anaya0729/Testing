# Use official Python image
FROM python:3.12.1

# Set working directory
WORKDIR /app

# Copy app code
COPY app.py .

# Install Flask directly via pip
RUN pip install flask

# Expose port
EXPOSE 5000

# Run the app
CMD ["python", "app.py"]
