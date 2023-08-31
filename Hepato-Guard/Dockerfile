# Menggunakan citra dasar yang sesuai dengan kebutuhan Anda
FROM python:3.11

# Menambahkan perintah untuk membangun lingkungan virtual dan menginstal dependensi
RUN python -m venv --copies /opt/venv && \
    . /opt/venv/bin/activate && \
    pip install --no-cache-dir -r requirements.txt

# Perintah lain yang mungkin Anda perlukan dalam konteks aplikasi Anda
# ...

# Menentukan direktori kerja di dalam kontainer
WORKDIR /app

# Menyalin aplikasi Anda ke dalam kontainer
COPY . /app

# Perintah yang akan dijalankan saat kontainer dimulai
CMD ["python", "app.py"]
