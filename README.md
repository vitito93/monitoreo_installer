# Monitoreo Installer 📲

Este repositorio contiene todo lo necesario para instalar la app **Monitoreo de Patentes** como **Device Owner** en un dispositivo Android.

---

## 🔧 Requisitos

- Un dispositivo Android **reseteado de fábrica**
- Una PC con Windows
- Cable USB
- Este repositorio descargado (no hace falta Android Studio)

---

## 📥 Descarga del instalador

1. Hacé clic en el botón **"Code" > Download ZIP**
2. Extraé el contenido en una carpeta (por ejemplo `C:\monitoreo_installer`)
3. Conectá el dispositivo por USB

---

## 🛠️ Instalación como Device Owner (sin QR)

1. **Abrí una terminal (CMD o PowerShell)**
2. Navegá a la carpeta donde descomprimiste el repositorio, por ejemplo:

```bash
cd C:\monitoreo_installer
```

3. Ejecutá los siguientes comandos:

```bash
adb install monitoreo.apk
adb shell dpm set-device-owner com.luxetecnogames.monitoreopatentes/.MyDeviceAdminReceiver
```