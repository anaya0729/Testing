# ---------- Stage 1: Build and install dependencies ----------
FROM python:3.12.1 AS builder
WORKDIR /app
RUN pip install --prefix=/install flask

# ---------- Stage 2: Final image ----------
FROM python:3.12.1
WORKDIR /app
COPY --from=builder /install /usr/local
COPY app.py .
EXPOSE 5000
CMD ["python", "app.py"]
