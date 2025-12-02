# Level Up Gamer - Tienda de Componentes de PC (App Android)

Esta es una aplicación de Android para una tienda ficticia de componentes de PC llamada "Level Up Gamer". La aplicación permite a los usuarios explorar productos por categoría, añadirlos a un carrito de compras y simular un proceso de pago. El proyecto está desarrollado de forma nativa con Kotlin y Jetpack Compose, siguiendo las mejores prácticas de arquitectura de Android.

## ✨ Características Principales

-   📱 **Interfaz Moderna con Jetpack Compose:** Toda la UI está construida con el moderno toolkit declarativo de Android, lo que permite un desarrollo de interfaz de usuario rápido y reactivo.
-   📂 **Arquitectura MVVM + Repository:** Sigue un patrón de arquitectura limpio (Model-View-ViewModel) que separa las responsabilidades, facilita las pruebas y mejora el mantenimiento del código.
-   🛍️ **Catálogo de Productos:** Muestra productos organizados por categorías (Tarjetas Gráficas, Procesadores, etc.) utilizando datos simulados que simulan una fuente de datos real.
-   🛒 **Carrito de Compras Funcional:**
    -   Añadir productos al carrito.
    -   Aumentar, disminuir o eliminar la cantidad de cada producto.
    -   Ver el total de la compra actualizado en tiempo real.
    -   Simulación de proceso de pago (checkout) que vacía el carrito.
-   📍 **Integración con GPS:** Utiliza los servicios de localización del dispositivo para obtener la ubicación del usuario y la convierte en una dirección legible mediante una API de geocodificación inversa (Nominatim).

## 🛠️ Stack Tecnológico y Arquitectura

-   **Lenguaje:** [Kotlin](https://kotlinlang.org/)
-   **UI:** [Jetpack Compose](https://developer.android.com/jetpack/compose)
-   **Arquitectura:** MVVM, Patrón Repositorio
-   **Gestión de Estado:** `StateFlow` y `ViewModel`
-   **Asincronía:** Coroutines y Flow
-   **Navegación:** [Navigation Compose](https://developer.android.com/jetpack/compose/navigation)
-   **Networking:** [Retrofit](https://square.github.io/retrofit/) (para la geocodificación)
-   **Localización:** [Google Play Services - FusedLocationProviderClient](https://developers.google.com/location-context/fused-location-provider)
-   **Simulación de DAO:** Se utiliza un `DAO` falso en memoria para simular el comportamiento de una base de datos, manteniendo la arquitectura desacoplada y lista para una futura implementación con Room o una API real.

## 🚀 Cómo Empezar

Sigue estos pasos para clonar y ejecutar el proyecto en tu máquina local.

1.  **Clonar el repositorio:**
    ```bash
    git clone https://github.com/tu_usuario/ProyectoAppMovil.git
    ```
2.  **Abrir en Android Studio:**
    -   Abre Android Studio (versión recomendada: Iguana o superior).
    -   Selecciona `Open` y elige la carpeta del proyecto que acabas de clonar.
3.  **Sincronizar Gradle:**
    -   Android Studio debería sincronizar el proyecto automáticamente. Si no es así, haz clic en el icono del elefante de Gradle con una flecha azul (`Sync Project with Gradle Files`).
4.  **Ejecutar la aplicación:**
    -   Selecciona un emulador o un dispositivo físico y haz clic en el botón de `Run 'app'` (▶️).
