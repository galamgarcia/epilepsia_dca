# Epilepsia DCA

Aplicación Android desarrollada como Trabajo Fin de Grado (TFG), titulada **"Monitorización de pacientes con pulseras inteligentes"**. Su objetivo es apoyar la monitorización de personas dependientes con daño cerebral adquirido (DCA) mediante la detección de posibles ataques epilépticos y el envío de alertas configurables a sus cuidadores.

**Autora:** Gala M. García Sánchez  
**Tutor:** José García Rodríguez  
**Curso académico:** 2015-2016  
**Fecha de publicación de la memoria:** 8 de octubre de 2016

## Enlaces

- [Página del proyecto](https://galamgarcia.github.io/epilepsia_dca/)
- [Memoria del TFG en el Repositorio Institucional de la Universidad de Alicante](https://rua.ua.es/entities/publication/1e5660cc-f1ce-48e6-8d6a-47b70f04587b)

## Objetivo

El proyecto explora el uso de una pulsera inteligente para la monitorización continua de constantes vitales y la mejora de la autonomía de pacientes con DCA. La aplicación se conecta mediante Bluetooth a una pulsera Angel Sensor, analiza los valores recibidos y genera una alerta cuando el ritmo cardiaco permanece fuera del rango configurado durante el tiempo establecido por la persona cuidadora.

La solución permite configurar notificaciones en el dispositivo y avisos SMS a un teléfono de emergencia. También muestra información de conexión, batería, señal, ritmo cardiaco y temperatura.

## Funcionalidades

- Registro, inicio de sesión y edición del perfil de usuario.
- Búsqueda y conexión Bluetooth con una pulsera Angel Sensor.
- Visualización de ritmo cardiaco, temperatura, batería y potencia de señal.
- Configuración de los límites mínimo y máximo de frecuencia cardiaca y del tiempo de espera para la alerta.
- Alertas mediante notificación local y/o SMS a un contacto de emergencia.
- Persistencia local de usuarios y configuración mediante SQLite.

## Tecnologías

- Android nativo con Java.
- Android SDK 24 y Android Gradle Plugin 2.1.2.
- Compatibilidad mínima: Android 4.3 (API 18).
- Gradle 2.10 mediante Gradle Wrapper.
- Bluetooth Low Energy y SDK de Angel Sensor.
- SQLite.

## Estructura

```text
Android/
  app/                 Aplicación Android
  angel-sdk-debug/     SDK de Angel Sensor usado por la aplicación
  angel-sdk-release/   Biblioteca de Angel Sensor incluida en el repositorio
  gradle/              Gradle Wrapper
```

## Compilación

El proyecto se conserva con la configuración de Android y Gradle empleada durante el TFG. Para abrirlo, importe el directorio `Android/` en una versión de Android Studio compatible con Android Gradle Plugin 2.1.2 y ejecute:

```bash
./gradlew assembleDebug
```

La aplicación usa el módulo `angel-sdk-debug` incluido en el repositorio.

## Alcance y advertencia

Este repositorio corresponde a un proyecto académico de 2016 y se publica con fines formativos y de investigación. No sustituye la supervisión médica ni constituye un producto sanitario certificado. Sus alertas no deben utilizarse como único mecanismo para tomar decisiones clínicas o de emergencia.

## Palabras clave

Daño cerebral adquirido, pulseras inteligentes, epilepsia, monitorización, eSalud, aplicación e Internet de las Cosas.

## Licencia

El código se distribuye bajo la [GNU General Public License v3.0](LICENSE).
