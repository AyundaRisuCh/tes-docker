## Buat Struktur Folder
project/

├── terraform/

│   ├── main.tf

├── register-app/

│   ├── app.py

│   ├── requirements.txt

│   └── Dockerfile

```bash
cd terraform
terraform init
terraform plan
terraform apply
```

sudo systemctl status docker

### Jika belum aktif
```bash
sudo systemctl start docker
sudo systemctl enable docker
```

### Cek apakah phpmyadmin sudah jalan
```bash
sudo docker ps
```

### Jika Belum
```bash
sudo docker run -d --name phpmyadmin \
  -e PMA_HOST=<ENDPOINT_RDS> \
  -e PMA_PORT=3306 \
  -e COOKIE_SECURE=false \
  -p 80:80 \
  phpmyadmin/phpmyadmin
```

