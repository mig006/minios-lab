# Resumen del proyecto

## De que trata

Este proyecto (miniOS) es un simulador educativo que explica, de forma simple, como un sistema operativo reparte el tiempo de la CPU entre varios programas. La idea es que el sistema actua como un "organizador": deja correr un programa un ratito, lo pausa, y luego le da turno a otro, repitiendo el ciclo para que todos avancen de manera justa.

Aunque es un simulador, usa programas reales del sistema. Es decir, cuando se lanza un programa desde la consola, se crea un proceso real, se detiene, y despues el sistema lo reanuda cuando le toca su turno. Esto permite observar el comportamiento de forma concreta, no solo teorica.

El sistema incluye una consola con comandos faciles para lanzar programas, ver en que estado estan y detenerlos. Ademas, tiene un panel web que muestra lo que pasa en tiempo real con graficas y contadores, para que sea mas visual. En el panel se ve una linea de tiempo que alterna los procesos, una tabla con estados, y algunas metricas basicas de uso.

## Lo que hice como estudiante

- Complete las partes faltantes del nucleo que permiten iniciar programas, pausar y reanudar turnos, y limpiar cuando un programa termina. Esto es lo que hace que el reparto del tiempo funcione en ciclos.
- Habilite los comandos del miniShell para ejecutar procesos, listar el estado, terminar un proceso y ver estadisticas generales. Sin estos comandos no seria posible controlar el simulador desde la consola.
- Ajuste el flujo para que, al crear el primer proceso, el sistema empiece a trabajar automaticamente y, cuando los procesos terminan, se liberen correctamente.
- Integre todo con las herramientas ya dadas del proyecto, de manera que el simulador funcione de principio a fin y se pueda observar en la consola y en el panel web.
