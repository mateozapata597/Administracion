# Administracion
esta es para la administración de la empresa

Sistema Administrativo S&H - Gestión Interna
Este es el panel de control administrativo de S&H. Desarrollamos esta herramienta interna para organizar toda la operación de la empresa, desde el seguimiento de obras hasta el manejo de inventario y personal.
¿Qué puede hacer el sistema?
El sistema está dividido en varios módulos, cada uno diseñado para resolver una necesidad específica de la administración:
1. Gestión de Proyectos (proyectos.html)
Es el corazón operativo. Permite registrar cada obra con su ID, estado y detalles.
•	Interactividad: Usamos ventanas modales para mostrar información detallada sin saturar la tabla principal.
2. Personal y Seguridad Social (personal.html)
Aquí gestionamos al equipo. Además de registrar datos, incluimos una funcionalidad para cargar y descargar documentos (como soportes de seguridad social) usando FileReader, lo que permite manejar archivos directamente en el navegador.
3. Contabilidad y Reportes (contabilidad_y_reportes.html)
Diseñamos un menú rápido para acceder a tareas contables frecuentes mediante tarjetas interactivas que facilitan el acceso a las funciones financieras.
4. Inventario y Proveedores (inventario.html)
Mantenemos el control de los materiales. Permite registrar productos, cantidades y precios, además de llevar un control de los proveedores que suministran los insumos.
5. Gestión de Roles (index.html)
Es la pantalla de inicio donde gestionamos los usuarios del sistema. Podemos agregar colaboradores y asignar roles, asegurando que cada persona tenga su registro actualizado.
¿Cómo funciona técnicamente?
•	Almacenamiento Local (LocalStorage): No necesitamos una base de datos externa. Toda la información (proyectos, empleados, inventario) se guarda directamente en el navegador del usuario usando localStorage. Esto hace que el sistema sea rápido y funcione sin necesidad de configurar un servidor.
•	Interfaz Unificada: Todos los archivos usan style.css y comparten una barra lateral (sidebar) para que la navegación entre módulos sea constante y sencilla.
•	Tablas Dinámicas: Usamos funciones de JavaScript para crear y editar filas en tiempo real. Esto permite que el administrador actualice datos (como cambiar el estado de un proyecto o modificar un precio) sin tener que recargar todo el sistema manualmente.
Proceso de desarrollo
1.	Diseño de Interfaz: Creamos un entorno sobrio y profesional usando tonos rojizos corporativos, asegurando que el espacio de trabajo fuera cómodo para el administrador.
2.	Programación Funcional: Nos enfocamos en que cada formulario fuera capaz de capturar datos y enviarlos a la memoria del navegador.
3.	Manejo de archivos: La gestión de documentos PDF, lo cual logramos resolviéndolo mediante la conversión de archivos a formato Base64 para su persistencia.
