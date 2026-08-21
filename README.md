# Epilepsia DCA

[English](README.md) | [Español](README.es.md)

Android application developed as an undergraduate final project, titled **"Monitoring patients with smart bands"**. Its purpose is to support the monitoring of dependent people with acquired brain injury (ABI) by detecting possible epileptic seizures and sending configurable alerts to their caregivers.

**Author:** Gala M. García Sánchez
**Supervisor:** José García Rodríguez
**Academic year:** 2015-2016
**Project report publication date:** October 8, 2016

## Links

- [Project page](https://galamgarcia.github.io/epilepsia_dca/)
- [Undergraduate project report in the University of Alicante Institutional Repository](https://rua.ua.es/entities/publication/1e5660cc-f1ce-48e6-8d6a-47b70f04587b)

## Purpose

The project explores the use of a smart band for the continuous monitoring of vital signs and for improving the autonomy of patients with ABI. The application connects to an Angel Sensor band over Bluetooth, analyzes the received values, and generates an alert when the heart rate remains outside the configured range for the period set by the caregiver.

The solution allows device notifications and SMS alerts to an emergency phone number to be configured. It also displays connection, battery, signal, heart rate, and temperature information.

## Features

- User registration, sign-in, and profile editing.
- Bluetooth discovery and connection to an Angel Sensor band.
- Display of heart rate, temperature, battery level, and signal strength.
- Configuration of the minimum and maximum heart rate thresholds and the alert delay.
- Alerts through a local notification and/or SMS to an emergency contact.
- Local persistence of users and settings with SQLite.

## Technologies

- Native Android with Java.
- Android SDK 24 and Android Gradle Plugin 2.1.2.
- Minimum compatibility: Android 4.3 (API 18).
- Gradle 2.10 through the Gradle Wrapper.
- Bluetooth Low Energy and Angel Sensor SDK.
- SQLite.

## Structure

```text
Android/
  app/                 Android application
  angel-sdk-debug/     Angel Sensor SDK used by the application
  angel-sdk-release/   Angel Sensor library included in the repository
  gradle/              Gradle Wrapper
```

## Building

The project is preserved with the Android and Gradle configuration used for the undergraduate project. To open it, import the `Android/` directory into a version of Android Studio compatible with Android Gradle Plugin 2.1.2, then run:

```bash
./gradlew assembleDebug
```

The application uses the `angel-sdk-debug` module included in the repository.

## Scope and disclaimer

This repository is an academic project from 2016 and is published for educational and research purposes. It does not replace medical supervision or constitute a certified medical device. Its alerts must not be used as the sole mechanism for making clinical or emergency decisions.

## Keywords

Acquired brain injury, smart bands, epilepsy, monitoring, eHealth, application, and Internet of Things.

## License

The code is distributed under the [GNU General Public License v3.0](LICENSE).
