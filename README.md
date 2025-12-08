🎯 Descripción del Proyecto
Sistema de Gestión de Recetario Personal es una aplicación desarrollada en C++ que permite organizar y gestionar recetas de cocina de manera digital. Este proyecto fue creado como parte de un trabajo académico para aplicar conceptos de programación orientada a objetos, estructuras de datos y manejo de archivos en un contexto real y útil.

El sistema implementa un modelo completo de recetario con funcionalidades avanzadas como clasificación por categorías, búsqueda inteligente, tipos especializados de recetas y persistencia robusta de datos. Todo el código sigue estándares profesionales de estilo, documentación y buenas prácticas de programación.

🏗️ Arquitectura Técnica
El proyecto está estructurado utilizando principios SOLID y sigue un diseño orientado a objetos con:

5 clases principales con relaciones claras

Herencia para especialización de tipos de recetas

Composición para manejo de ingredientes y recetas

Polimorfismo para operaciones comunes

Persistencia robusta en formato CSV con manejo de caracteres especiales

✅ Para qué SIRVE este sistema
🍳 Funcionalidades Principales
1. Gestión Completa de Recetas
Creación: Agregar recetas con todos sus detalles (nombre, categoría, tiempo, instrucciones)

Organización: Clasificar recetas por categorías personalizadas

Almacenamiento: Guardado automático en archivo CSV

Modificación: Edición y actualización de recetas existentes

2. Tipos Especializados de Recetas
Recetas Base: Recetas generales sin restricciones

Recetas Saludables: Con información de calorías y opción vegana

Recetas Rápidas: Con nivel de dificultad para preparaciones exprés

3. Sistema de Búsqueda Avanzado
Búsqueda por nombre: Encuentra recetas por nombre completo o parcial

Búsqueda insensible: No distingue entre mayúsculas y minúsculas

Listado completo: Visualiza todas las recetas con resumen

4. Gestión de Ingredientes
Lista detallada de ingredientes con cantidades y unidades

Múltiples ingredientes por receta

Formato claro para lectura y preparación

5. Persistencia Robusta
Guardado automático: Al salir del programa

Carga automático: Al iniciar el programa

Formato CSV seguro: Maneja comas, comillas y saltos de línea

Tolerancia a errores: No se corrompe con datos inválidos

6. Interfaz de Usuario Intuitiva
Menús jerárquicos claros

Validación de entrada de datos

Confirmaciones antes de operaciones destructivas

Formato de salida profesional y legible

❌ Para qué NO SIRVE este sistema
Limitaciones Intencionales del Proyecto
1. NO es una aplicación multiusuario o en red
Solo un usuario por instancia del programa
No tiene sistema de autenticación o perfiles
No sincroniza datos entre dispositivos

2. NO tiene interfaz gráfica (GUI)
Es una aplicación de consola/terminal
No incluye imágenes o elementos gráficos
Requiere ejecución en línea de comandos

3. NO maneja características avanzadas de cocina
No calcula valores nutricionales automáticamente
No convierte unidades de medida (tazas a gramos, etc.)
No genera listas de compras automáticas
No planifica menús semanales

4. NO es un sistema de compartición
No exporta a formatos para impresión bonita
No comparte recetas en redes sociales
No tiene integración con sitios web de recetas

5. NO tiene funcionalidades de red o nube
No se conecta a internet para buscar recetas
No hace respaldos automáticos en la nube
No tiene sistema de actualizaciones automáticas

6. Limitaciones técnicas específicas
No maneja miles de recetas simultáneamente (diseñado para uso personal)
No tiene sistema de etiquetas múltiples por receta
No incluye temporizador de cocina integrado

🛠️ Cómo USAR el sistema
Requisitos Previos
Para usar este programa necesitas tener instalado un compilador de C++ compatible como g++, clang++ o MSVC, y acceso a una terminal o consola de comandos. El sistema funciona en Windows, Linux y macOS sin modificaciones adicionales.

Instalación y Compilación
Primero crea un directorio para el proyecto y guarda el código fuente en un archivo llamado recetario.cpp. Para compilar, abre tu terminal y ejecuta el comando correspondiente a tu sistema operativo. En Linux o macOS usa: g++ -o recetario recetario.cpp -std=c++11. En Windows con MinGW usa: g++ -o recetario.exe recetario.cpp -std=c++11. Si estás usando Visual Studio en Windows, el comando es: cl recetario.cpp /EHsc /std:c++11. Una vez compilado, en Linux/macOS ejecuta con ./recetario y en Windows con recetario.exe.

Primer Uso y Configuración
Al ejecutar el programa por primera vez, verás un mensaje indicando que no se encontró archivo de recetas previo y se creará uno nuevo. Aparecerá el menú principal con 8 opciones numeradas. El sistema creará automáticamente un archivo llamado recetas.csv en el mismo directorio donde está el ejecutable, que contendrá todas tus recetas guardadas.

Menú Principal y Navegación
El menú principal muestra las siguientes opciones: 1) Agregar nueva receta, 2) Listar todas las recetas, 3) Buscar receta por nombre, 4) Agregar receta saludable, 5) Agregar receta rápida, 6) Ver detalles de receta, 7) Eliminar receta, y 8) Salir. Para seleccionar una opción, simplemente ingresa el número correspondiente y presiona Enter. El sistema validará que tu entrada sea correcta y te guiará a través de cada proceso.

Agregar una Nueva Receta
Al seleccionar la opción 1 para agregar una receta básica, el sistema te pedirá: el nombre de la receta (ej: "Ensalada César"), la categoría (ej: "Ensalada"), el tiempo de preparación en minutos (ej: 20). Luego te pedirá las instrucciones: escribe cada paso en una línea separada y cuando termines escribe "fin" en una línea nueva. Después agregarás ingredientes: para cada ingrediente proporciona el nombre (ej: "Lechuga romana"), la cantidad (ej: "1") y la unidad (ej: "cabeza"). Puedes agregar tantos ingredientes como necesites. Finalmente, el sistema confirmará que la receta fue agregada exitosamente.

Crear Recetas Especializadas
Si seleccionas la opción 4 para receta saludable, seguirás el mismo proceso que para una receta básica pero adicionalmente te pedirá las calorías por porción (ej: 150) y si la receta es vegana (responde s/n). Para recetas rápidas (opción 5), además de los datos básicos te pedirá un nivel de dificultad del 1 al 5, donde 1 es muy fácil y 5 es más complejo pero rápido de preparar.

Buscar y Visualizar Recetas
Para buscar una receta (opción 3), ingresa parte o todo el nombre de la receta que buscas. El sistema mostrará todas las recetas cuyo nombre contenga el texto que ingresaste, sin importar mayúsculas o minúsculas. Para ver el detalle completo de una receta específica, primero selecciona la opción 2 para listar todas las recetas, anota el número que aparece junto a la receta que te interesa, luego selecciona la opción 6 e ingresa ese número. Verás todos los detalles incluyendo ingredientes, tiempo, categoría e instrucciones completas.

Gestionar y Eliminar Recetas
Para eliminar una receta, primero usa la opción 2 para listar todas las recetas y anota el número de la receta que deseas eliminar. Luego selecciona la opción 7, ingresa el número de la receta y confirma la eliminación escribiendo "s" cuando se te pregunte. El sistema te pedirá confirmación antes de proceder para evitar eliminaciones accidentales.
