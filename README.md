# Centro de Impresión 3D - Plataforma Web

Bienvenido al repositorio oficial del **Centro de Impresión 3D**, una plataforma web diseñada para ofrecer servicios locales de impresión 3D de manera profesional, rápida y automatizada.

## 🚀 Descripción del Proyecto

Esta página web actúa como el escaparate principal y el punto de entrada para los clientes que desean materializar sus ideas. Permite a los usuarios buscar modelos 3D, conocer el proceso de impresión, revisar la tecnología utilizada y gestionar su inicio de sesión, todo en una interfaz moderna y responsiva.

## ✨ Funcionalidades Principales

* **Búsqueda Integrada (Thingiverse):** Los usuarios pueden buscar diseños listos para imprimir directamente desde la página principal, redirigiéndolos a una galería conectada a la API de Thingiverse.
* **Autenticación Segura:** Sistema de inicio de sesión integrado con **Google OAuth** a través de Supabase, permitiendo a los usuarios acceder a su panel de control personalizado (`dashboard.html`).
* **Estado de Hardware en Tiempo Real:** La sección de tecnología consulta una base de datos en tiempo real (Supabase) para mostrar el filamento que la impresora (Creality Ender-3 S1 Pro) está utilizando en ese momento exacto.
* **Widget de Clima Local:** Un componente interactivo y expandible que obtiene el clima en tiempo real de la ciudad de operaciones (Calama) usando **WeatherAPI**.
* **Conversor de Divisas Dinámico:** Un widget integrado en la interfaz que permite a los usuarios convertir precios entre CLP (Pesos Chilenos), USD y EUR, consumiendo datos oficiales y en tiempo real del Banco Central a través de la API de **Mindicador.cl**.
* **Galería y Multimedia:** Visualización interactiva de la maquinaria con intercambio de imágenes y enlace al tráiler oficial en video de la impresora.

## 🛠️ Tecnologías y Herramientas Utilizadas

* **Frontend:** HTML5, CSS3 (Variables, CSS Grid, Flexbox), JavaScript (Vanilla).
* **Backend & Base de Datos:** [Supabase](https://supabase.com/) (Autenticación y PostgreSQL).
* **APIs Externas:**
    * `WeatherAPI` (Datos meteorológicos en tiempo real).
    * `Mindicador.cl` (Valores oficiales de divisas en Chile).
    * `Thingiverse.com` (Centro de modelos para Impresión 3D)
    * `Autenticación de Google` (Ingreso al sistema rápido con Google)
* **Iconografía:** FontAwesome 6.0.

## 📂 Estructura Principal

* `index.html`: Landing page principal con toda la información del servicio y widgets.
* `ModelosThingiverse.html`: Página encargada de mostrar los resultados de búsqueda de modelos 3D.
* `dashboard.html`: Panel de control al que accede el usuario tras iniciar sesión con Google.
* `login.html`: Interfaz alternativa de autenticación.
* `css/style.css`: Hoja de estilos principal.

## ⚙️ Cómo ejecutar el proyecto

Dado que el proyecto utiliza tecnologías web estándar (HTML, CSS, JS), no requiere un servidor backend complejo para su visualización básica:

1. Clona este repositorio o descarga los archivos.
2. Abre el archivo `index.html` en cualquier navegador web moderno.
3. *Nota:* Para que la autenticación de Google y la lectura del filamento funcionen correctamente en un entorno local, asegúrate de estar ejecutando el proyecto a través de un servidor local (por ejemplo, la extensión *Live Server* de VS Code) debido a las políticas de CORS de Supabase y las APIs.

## 👤 Autor

Proyecto desarrollado como parte de una solución integral para servicios de impresión 3D.
