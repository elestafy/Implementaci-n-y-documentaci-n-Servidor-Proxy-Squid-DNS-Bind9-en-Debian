#!/bin/bash

echo " Instalando y configurando Bind9..."

sudo apt update && sudo apt install -y bind9 bind9utils dnsutils

# Copiar archivos de configuración (asume que estás en la raíz del repo)
sudo cp bind/named.conf.options /etc/bind/
sudo cp bind/named.conf.local /etc/bind/
sudo cp bind/db.tudominio.local /etc/bind/
sudo cp bind/db.192.168.147 /etc/bind/

# Verificar sintaxis
sudo named-checkconf
sudo named-checkzone tudominio.local /etc/bind/db.tudominio.local
sudo named-checkzone 147.168.192.in-addr.arpa /etc/bind/db.192.168.147

# Reiniciar
sudo systemctl restart bind9
sudo systemctl enable bind9
