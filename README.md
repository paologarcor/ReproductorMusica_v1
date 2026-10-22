# ReproductorMusica

**ReproductorMusica** es una aplicación móvil nativa para Android desarrollada en Kotlin, diseñada con tecnologías modernas de UI como **Jetpack Compose** y el sistema de diseño **Material 3**.

---

## Características Principales

- **UI Declarativa Moderna:** Construida íntegramente con [Jetpack Compose](https://developer.android.com/jetpack/compose).
- **Material 3:** Implementación de temas personalizados (`Theme.kt`, `Color.kt`, `Type.kt`) siguiendo las últimas directrices de diseño de Android.
- **Edge-to-Edge:** Soporte nativo para inmersión visual con `enableEdgeToEdge()` en barras de navegación y estado.
- **Arquitectura Limpia y Escalable:** Estructura modularizada lista para la implementación de patrones MVVM y servicios multimedia.

---

## Tecnologías y Dependencias

- **Lenguaje:** Kotlin
- **UI Toolkit:** Jetpack Compose (BOM gestionado)
- **Componentes:**
  - `androidx.core:core-ktx`
  - `androidx.lifecycle:lifecycle-runtime-ktx`
  - `androidx.activity:activity-compose`
  - `androidx.compose.material3:material3`
- **Configuración SDK:**
  - **Min SDK:** 24 (Android 7.0 Nougat)
  - **Compile/Target SDK:** 36

---

## Estructura del Proyecto

```text
ReproductorMusica/
├── app/
│   ├── build.gradle.kts                # Configuración de dependencias y compilación del módulo
│   └── src/
│       └── main/
│           ├── AndroidManifest.xml     # Manifiesto de la aplicación y declaración de actividades
│           └── java/
│               └── com/example/reproductormusica/
│                   ├── MainActivity.kt # Actividad principal de entrada con Compose
│                   └── ui/
│                       └── theme/      # Definiciones de Material 3 (Color, Theme, Type)
└── build.gradle.kts                    # Configuración raíz del proyecto
```

---

## Primeros Pasos y Compilación

1. **Clonar o abrir el repositorio** en [Android Studio](https://developer.android.com/studio).
2. Sincronizar el proyecto con Gradle (`File > Sync Project with Gradle Files`).
3. Ejecutar la aplicación en un dispositivo físico o emulador con **Android 7.0 (API 24)** o superior.

---

## Roadmap / Próximas Funcionalidades

- [ ] Integración con **Jetpack Media3 / ExoPlayer** para la reproducción de archivos de audio locales y en streaming.
- [ ] Gestión de permisos de archivos multimedia (`READ_MEDIA_AUDIO` / `READ_EXTERNAL_STORAGE`).
- [ ] Explorador de canciones, álbumes y artistas.
- [ ] Controles de reproducción en segundo plano (Notificación multimedia con `MediaSession`).
- [ ] Pantalla de reproducción en curso (*Now Playing*).
