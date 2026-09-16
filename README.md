🚀 Demo de conexión con OpenAI (Key Authentication)
Este proyecto es una demostración sencilla de cómo conectarse a la API de OpenAI usando Python, autenticación por API Key y variables de entorno para mantener las credenciales seguras. El script realiza una consulta al modelo y muestra la respuesta generada en consola.

📦 Características principales
🔐 Autenticación por API Key usando variables de entorno.
🌱 Carga automática de .env con python-dotenv.
🤖 Solicitud al modelo gpt-5-mini mediante client.responses.create().
🖥️ Ejecución simple y salida clara en consola.
📁 Código minimalista ideal para aprendizaje o integración en proyectos más grandes.

🧠 Estructura del proyecto
Code
📂 proyecto-openai-demo
 ├── demo.py
 ├── .env
 ├── README.md

⚙️ Requisitos
Python 3.9+

Librerías:
openai
python-dotenv

Instalación:
bash
pip install openai python-dotenv

🔧 Configuración
Crea un archivo .env en la raíz del proyecto:
env
url_endpoint=https://api.openai.com/v1
api_key=TU_API_KEY_AQUI

▶️ Ejecución
Ejecuta el script:
bash
python demo.py

🧩 ¿Cómo funciona?
Componente	Función
load_dotenv()	Carga las variables del archivo .env.
os.getenv()	Obtiene api_key y url_endpoint.
OpenAI()	Inicializa el cliente con autenticación por API Key.
client.responses.create()	Envía la pregunta al modelo y recibe la respuesta.
print()	Muestra la respuesta generada.


📤 Ejemplo de salida
Code
answer: The capital of France is Paris.

🛡️ Seguridad
Este proyecto utiliza Key Authentication, lo que significa que tu clave privada nunca debe incluirse directamente en el código.
El uso de .env evita exponer credenciales en GitHub o en despliegues.

📚 Recursos útiles
Documentación de OpenAI
Variables de entorno con python-dotenv
Modelos GPT y respuestas