# Laboratorio de DMZ con Cisco Packet Tracer

## Objetivo
El objetivo de este laboratorio es configurar una zona desmilitarizada (DMZ) en un router Cisco, aplicando NAT estático y ACLs para controlar el tráfico entre LAN, DMZ y red externa.  
Se busca exponer un servidor web de manera segura, permitiendo acceso desde Internet únicamente por HTTP, bloqueando tráfico no autorizado desde la DMZ hacia la LAN y asegurando conectividad interna.

## Contenidos del repositorio
- Informe_DMZ_Laboratorio.pdf → Documento con la explicación completa de la topología, direccionamiento, configuración aplicada y pruebas realizadas.  
- PacketTracer.pka → Archivo de simulación en Cisco Packet Tracer con la topología implementada.  
- Evidencias.pdf → Archivo con evidencias de las pruebas (pings, navegador y comandos).  
- README.md → Este archivo, con la descripción general del laboratorio y del repositorio.

## Topología
- LAN (192.168.1.0/24): PC_Internal y switch interno.  
- DMZ (192.168.2.0/24): Servidor web expuesto.  
- Externa (192.168.3.0/24): PC_External simulando Internet.  
- Router_FW: Cisco que conecta las tres zonas, aplica NAT y ACLs.

## Resultados esperados
- LAN → DMZ: acceso permitido.  
- Internet → DMZ: acceso permitido solo por HTTP.  
- DMZ → LAN: acceso bloqueado. 
