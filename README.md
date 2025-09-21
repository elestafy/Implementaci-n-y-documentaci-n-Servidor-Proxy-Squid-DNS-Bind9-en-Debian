# Implementaci-n-y-documentaci-n-Servidor-Proxy-Squid-DNS-Bind9-en-Debian
S8 Napo


Repositorio: Configuración DNS + Proxy (Bind9 + Squid)

Equipo Tonotos — Laboratorio de Redes



Objetivo

Este repositorio contiene los archivos de configuración originales y scripts para restaurar rápidamente la infraestructura de DNS (Bind9) y Proxy (Squid) en Debian 12.



 Requisitos previos

- Máquina Debian 12 (VM o física)
- IP estática configurada: `192.168.147.128`
- Interfaz de red: `ens33`
- Acceso root o sudo


 Estructura del repositorio

- `bind/` → Archivos de configuración de Bind9
- `squid/` → Archivo de configuración de Squid
- `scripts/` → Scripts de instalación automática
- `docs/` → Bitácora y diagrama de red



Cómo restaurar la configuración

 1. Instalar servicios (opcional: usar scripts)

bash
sudo ./scripts/install_bind.sh
sudo ./scripts/install_squid.sh
