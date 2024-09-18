# Gunakan gambar dasar
FROM python:3.11.9

# Atur direktori kerja
WORKDIR /app

# Pasang dependensi
RUN pip install fastapi uvicorn

# Salin file main.py ke direktori kerja /app
COPY ./main.py /app/
COPY data /app/data

# Jalankan aplikasi
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
