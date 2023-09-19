# JetAReader
Aprendizajes:

1. `package com.bawp.freader`: Esto define el paquete en el que se encuentra la clase `MainActivity`.

2. `import`: En esta sección se importan las clases y paquetes necesarios para la aplicación.

3. `@ExperimentalComposeUiApi`: Esto es una anotación que indica que la actividad hace uso de características experimentales de Compose UI.

4. `@AndroidEntryPoint`: Esta anotación se utiliza en conjunción con Hilt (un marco de inyección de dependencias para Android) para indicar que esta actividad debe ser inyectada automáticamente con las dependencias proporcionadas por Hilt.

5. `class MainActivity : ComponentActivity()`: Aquí se define la clase `MainActivity` como una subclase de `ComponentActivity`, que es una clase de Android Jetpack utilizada para actividades de Compose.

6. `override fun onCreate(savedInstanceState: Bundle?)`: Este es el método `onCreate` de la actividad, que se llama cuando la actividad se crea por primera vez.

7. `setContent`: Esto configura el contenido de la actividad utilizando Compose. En este caso, se establece el tema de la aplicación como `FReaderTheme` y se llama a la función `ReaderApp()` para establecer la interfaz de usuario de la aplicación.

8. `@Composable fun ReaderApp()`: Aquí se define una función composable llamada `ReaderApp`. Los componibles son funciones que definen partes de la interfaz de usuario de la aplicación. En este caso, `ReaderApp` define la estructura principal de la interfaz de usuario.

9. `Surface`: `Surface` es un componente de Compose que define un área rectangular con un color de fondo. En este caso, se utiliza para definir la superficie de la pantalla principal de la aplicación. Se le pasa el color de fondo del tema de Material Design y se especifica que debe ocupar toda la pantalla (`fillMaxSize()`).

10. `Column`: `Column` es otro componente de Compose que organiza sus hijos en una columna vertical. En este caso, se utiliza para colocar el contenido en el centro de la pantalla tanto vertical como horizontalmente. Dentro de la columna, se llama a `ReaderNavigation()`, que probablemente define la navegación de la aplicación.

11. `@Preview`: Esto define una función composable de vista previa utilizada en el entorno de desarrollo para previsualizar cómo se vería el tema `FReaderTheme`. Esta función no se utiliza en la aplicación en tiempo de ejecución, pero es útil para fines de desarrollo.

