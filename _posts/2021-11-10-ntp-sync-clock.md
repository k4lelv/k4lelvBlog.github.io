---

layout: single
title: Como Sincronizar hora con NTP en Linux
date: 2021-11-10
classes: wide
header:
    teaser: /assets/images/slae32.png
categories:
    - utilidades
    - linux
tags:
    - utilidades
    - linux
    - sync
    - automatizacion

---
<p align = "Center">
    <img src="/assets/images/ntpSync/imgNtpSync.jpg">
</p>

Uno de los comandos mas útiles en Linux es NTP (Network Time Protocol) el cual se encarga de sincronizar de forma automática la hora de nuestro [servidor en red](https://www.solvetic.com/page/recopilaciones/s/recopilacion/mejores-distribuciones-para-servidor-linux) y esto es un punto delicado cuando hablamos de un equipo en ambientes productivos ya que una mala sincronización de la hora puede llegar a afectar diversas tareas y mas si el equipo es un servidor.

El equipo puede hacer permitir que el reloj del sistema haga uso del Tiempo Universal Coordinado (UTC) en lugar de la hora local para estar mucho mas acorde a la hora requerida. Como administradores, la forma clásica de realizar la sincronización de la hora es haciendo uso del comando ntpdate, el cual se encarga de configurar la hora del sistema desde un servidor horario NTP establecido.

### Veamos como seria hacer uso de NTP en linux.
---------------
1. Instalamos NTP en nuestra maquina linux

```
sudo apt-get install ntpdate (Debian/Ubuntu)
sudo yu install ntpdate      (CentOS/RHEL)
sudo dnf install ntpdate     (Fedora)
```
