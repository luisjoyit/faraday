# security-pipelines

descargamos el faraday abrimos en el visual studio code el archivo yml y ponemos terminal y escribimos 

```bash
docker compose up
```


se nos instalara el faraday para el faraday en usuarios se es faraday y la contraseña aparece en docker enla parte faraday-app

para poder integrar manualmente las herraminetas 
[manual.pdf](https://github.com/user-attachments/files/18424763/manual.pdf)





NMAP

link de descarga https://nmap.org/

manual [nmap.pdf](https://github.com/user-attachments/files/18491187/nmap.pdf)


abres el terminal y escribes  y te apareceran los comando

nmap

Escaneo básico de un solo host:

nmap (ip)

Escaneo completo (todos los puertos):

```bash
nmap -p- (ip)

#Escaneo de puertos específicos:


nmap -p 80,443 (ip)

# Reporte en formato XML/html

nmap -oX reporte.xml (ip)   

nmap -oX reporte.html (ip)
```




NESSUS 

link de descarga https://www.tenable.com/downloads/nessus?loginAttempted=true

primero ponemos nessus esencial y rellenas lo que te pide

![1](https://github.com/user-attachments/assets/c3d860fe-354e-4e22-933a-de8023264ddf)

despues esperas q te cargen los pluyin 

manual[nessus.pdf](https://github.com/user-attachments/files/18491289/nessus.pdf)




OPENVAS

se descarga en un docker entoces primeor descagas docker y creas un contenedor 

par que tengas la imagen de openvas abres terminal

 ```bash
docker pull greenbone/gvm
```

Ejecutar OpenVAS con Docker

 ```bash
docker run -d -p 8080:9392 --name openvas greenbone/gvm
```

verificas

 ```bash
docker ps
```

manual [openvas.pdf](https://github.com/user-attachments/files/18491338/openvas.pdf)




ZAP

link de descarga https://www.zaproxy.org/download/


manual[zap.pdf](https://github.com/user-attachments/files/18491523/zap.pdf)


 Crear la carpeta de informes

 ```bash
 mkdir C:\Users\aa\zap_reports
```

 Definir la URL a analizar
  ```bash
set url=(url)
```
Ejecutar Docker con ZAP
 ```bash
docker run --rm --user root -v C:\Users\aa\zap_reports:/zap/wrk ghcr.io/zaproxy/zaproxy:stable zap-baseline.py -t "%url%" -r "C:\Users\aa\zap_reports\zap_report.html" -x "C:\Users\aa\zap_reports\zap_report.xml"
```


 





exel de las herramientas usadas 
[faraday.xlsx](https://github.com/user-attachments/files/18491553/faraday.xlsx)











