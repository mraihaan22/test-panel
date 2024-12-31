# Pterodactyl Panel in GitHub Codespaces

This repository provides a setup to run Pterodactyl Panel and Wings in GitHub Codespaces using Docker Compose.

## How to Run

1. Open this repository in GitHub Codespaces.
2. Run the following command to start the services:
   ```bash
   docker-compose up -d

3. Access the panel at http://<workspace-id>.github.dev:8080.



Notes

Persistent data is stored in panel_data/ and wings_data/.

Update docker-compose.yml to configure tokens for Wings.


---

### **3. Tips**
1. **Token Configuration**:
   Setelah membuat node di Panel, tambahkan `WINGS_TOKEN_ID` dan `WINGS_TOKEN_SECRET` ke file `docker-compose.yml`.

2. **Port Mapping**:
   - `8080` untuk Panel.
   - `2022` untuk Wings.

3. **Volume Configuration**:
   - Gunakan `./panel_data` dan `./wings_data` agar data tidak hilang saat container berhenti.