# 🤖 **UiPath Email Processor Bot** 📧

Este repositorio contiene un bot automatizado desarrollado con **UiPath** para procesar correos electrónicos de **Outlook**. El bot realiza las siguientes acciones:

---

## 🛠️ **Funcionalidad**

1. **Recorrido de correos electrónicos**: El bot revisa los correos de una cuenta de Outlook especificada y filtra los correos provenientes de un dominio específico (por defecto, **Gmail**).
   
2. **Descarga y descompresión de archivos ZIP**: Si el correo contiene un archivo ZIP, el bot lo descarga y lo guarda en una carpeta temporal. Luego, descomprime el archivo ZIP en una carpeta separada.

3. **Procesamiento de PDFs**: Los archivos ZIP descargados contienen exclusivamente archivos **PDF**. El bot combina estos PDFs en un solo documento.

4. **Exportación**: El archivo PDF combinado se guarda en una carpeta de **exportación** para su posterior uso.

---

## ⚠️ **Consideraciones**

- **Proceso específico**: Este bot está diseñado para un proceso específico, donde los archivos ZIP solo contienen **PDFs**. Si los archivos ZIP contienen otros tipos de archivos, el bot no los procesará correctamente.
- **Carpetas necesarias**: Asegúrate de crear las carpetas **"Import"** y **"Export"** antes de ejecutar el bot.
- **Permisos**: Verifica que tienes los permisos necesarios para ejecutar el bot correctamente y acceder a las carpetas de entrada y salida.
- **Sensibilidad a mayúsculas y minúsculas**: Asegúrate de ingresar los datos correctamente, ya que el bot es sensible a las mayúsculas y minúsculas.

---

## 📝 **Instrucciones**

1. **Preparación**: Crea las carpetas **"Import"** y **"Export"** en la ubicación que el bot pueda acceder.
2. **Ejecución**: Ejecuta el bot en **UiPath Studio**. El bot buscará correos con archivos ZIP adjuntos, los descargará y descomprimirá.
3. **Exportación**: Los PDFs de un mismo correo se combinarán en un solo archivo y se guardarán en la carpeta **"Export"**.

---

## 💻 **Lenguaje y tecnologías utilizadas**

- **UiPath**: Plataforma de automatización de procesos.
- **XAML**: Archivos de flujo de trabajo de UiPath.

---

## 🛠️ **Requisitos**

- **UiPath Studio**: Este proyecto debe ser ejecutado desde **UiPath Studio**.
- **Permisos**: Asegúrate de tener permisos para acceder a los correos electrónicos y las carpetas necesarias.

---

## 📜 **License**

Este proyecto está bajo la Licencia **MIT**. Consulta el archivo `LICENSE` para más detalles.


