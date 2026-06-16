# Examen-HTTP
# Instalacion ngix
sudo apt install nginx -y

# Creación de webs
sudo mkdir /var/www/web1
sudo mkdir /var/www/web2

sudo nano /var/www/web1/index.html
sudo nano /var/www/web2/index.html

sudo cp /etc/nginx/sites-available/default /etc/nginx/sites-available/web1
sudo cp /etc/nginx/sites-available/default /etc/nginx/sites-available/web2

# Configuración web 1
<img width="524" height="165" alt="image" src="https://github.com/user-attachments/assets/61478dc1-bb90-4e09-9687-2d650bba8241" />


# Configuración web 2
<img width="596" height="199" alt="image" src="https://github.com/user-attachments/assets/46e7d875-df4d-4dbe-a1fe-2eb01f96ed33" />

# Configuración web 1 mantenimiento
sudo mkdir /var/www/web1
sudo nano /var/www/web1.mantenimiento/index.html
<img width="647" height="133" alt="image" src="https://github.com/user-attachments/assets/c4542107-ac1e-428b-93e4-43d1afd81473" />


# Vinculo
sudo ln -s /etc/nginx/sites-available/web1 /etc/nginx/sites-enabled/
sudo ln -s /etc/nginx/sites-available/web2 /etc/nginx/sites-enabled/
sudo ln -s /etc/nginx/sites-available/web1.mantenimiento /etc/nginx/sites-enabled/

# Cliente interno
<img width="344" height="76" alt="image" src="https://github.com/user-attachments/assets/2442556d-a537-4a8b-92cb-1d51054c4864" />

# Redirecciónes
## web1
http://web1.org pasa a ser https://web1.org
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/2df8ff30-27ed-4137-b572-7f2df1a6f821" />

## web2
Aun no redirije pero al menos se ve que llega al servidor (ya que esta maquina no tiene acceso a internet al estar en una red interna)
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/160767a8-d4d3-4f2e-bbdf-e7e1d5f505af" />

