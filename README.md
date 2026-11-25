# Probador de SEO Movil y Experiencia Responsiva

[![Probador SEO Movil](https://img.shields.io/badge/TAVARDT-Mobile%20SEO-5b3cf5.svg)](https://tools.tavardt.com/mx/prueba-seo-movil/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Auditoria de compatibilidad mobile-first, parametros de viewport, anchuras fijas, legibilidad de fuentes y ergonomia tactil.

***

## Vectores de Riesgo e Impacto Operativo en Experiencia Movil

Los sitios web sin directivas de viewport correctas suspenden la indexacion mobile-first de Google y pierden posicionamiento en Mexico. Las fallas de diseno responsivo obligan al desplazamiento horizontal y provocan el abandono de los usuarios.

Bloquear la escala de zoom vulnera las normativas de accesibilidad web y afecta a usuarios con dificultades de vision. Las dimensiones fijas superiores al ancho de pantalla y las tipografias reducidas elevan la tasa de rebote.

***

## Capacidades Centrales de Auditoria Tecnica

* **Analisis de Directiva Viewport**: Comprueba la presencia de la meta etiqueta, ancho de dispositivo, escala inicial y bloqueo de zoom, deduciendo hasta 45 puntos si falta.
* **Deteccion de Desbordamiento Horizontal**: Identifica reglas CSS con anchos fijos superiores a 450px que provocan desplazamiento lateral en smartphones.
* **Auditoria de Legibilidad Tipografica**: Rastrea declaraciones de tamano de fuente inferiores a 12px, penalizando textos diminutos con hasta 15 puntos.
* **Cuantificacion de Objetivos Tactiles**: Mapea enlaces, botones y campos de formulario para verificar la ergonomia y densidad de toques.
* **Validacion de Icono Tactil (Apple Touch Icon)**: Revisa la inclusion de la etiqueta apple-touch-icon en el encabezado HTML, deduciendo 5 puntos si no se encuentra.
* **Indice de Ergonomia Movil**: Calcula una valoracion de 0 a 100 categorizada en SATISFACTORY, ADVISORY o UNSATISFACTORY.
* **Emulacion Movil Autentica**: Realiza solicitudes HTTP mediante un encabezado User-Agent genuino de Safari en iPhone para una evaluacion realista.

***

## Instalacion y Ejecucion

Requiere Python 3.8 o superior utilizando unicamente bibliotecas estandar.

```bash
git clone https://github.com/TAVARDT-Mexico/mobile-seo-tester-mx.git
cd mobile-seo-tester-mx
python mobile_seo_tester.py https://empresa.mx
```

Para generar la salida en formato estructurado JSON en procesos automatizados de auditoria:

```bash
python mobile_seo_tester.py https://empresa.mx -j
```

***

## Preguntas Frecuentes (FAQ Tecnico)

### 1. Como afecta la ausencia o mala configuracion de la etiqueta viewport a la indexacion movil?
Los motores de busqueda evaluan las paginas web emulando exclusivamente pantallas moviles. Sin la etiqueta viewport configurada con device-width, el navegador aplica la vista de escritorio y penaliza severamente el posicionamiento del sitio.

### 2. Por que se penaliza desactivar el zoom del usuario con la directiva user-scalable=no?
Impedir la ampliacion manual vulnera los principios de accesibilidad de la W3C para personas que requieren acercar el texto. Los algoritmos de busqueda registran el bloqueo de zoom como un fallo de usabilidad y disminuyen la calificacion tecnica.

### 3. Como perjudican los contenedores rigidos con anchos superiores a 450px a la navegacion movil?
Los elementos con anchos fijos mayores a 450px superan el tamano de pantalla de la mayoria de telefonos moviles y obligan al usuario a desplazarse hacia los lados. Esta rotura del diseno responsive ocasiona la suspension en las pruebas de optimizacion movil.

### 4. Que riesgos operativos conllevan las fuentes declaradas por debajo de 12px?
El texto de tamano inferior a 12px resulta dificil de leer en pantallas de alta densidad sin aplicar zoom constante. El analizador aplica deducciones para asegurar que los contenidos principales sean legibles de manera inmediata.

### 5. Por que es indispensable configurar el icono apple-touch-icon en la cabecera HTML?
El atributo apple-touch-icon permite que los sistemas operativos de moviles muestren un icono de marca nitido cuando el usuario anade la pagina a su pantalla de inicio. Omitir este enlace genera iconos por defecto poco profesionales que debilitan la presencia digital.

***

## Asesoria en SEO Movil y Arquitectura Adaptable

Para portales de alto trafico y cumplimiento riguroso de las directrices Google Mobile-First Indexing y W3C, consulte al equipo de **TAVARDT**.

***

## Enlaces Utiles

* **Portal Corporativo:** https://ag.tavardt.com/mx/
* **Suite de Diagnosticos:** https://tools.tavardt.com/mx/
* **Contacto Tecnico:** https://ag.tavardt.com/mx/contacto/

***

### Licencia
Distribuido bajo la Licencia MIT. Consulte el archivo LICENSE para mas detalles.

***

© 2026 TAVARDT. Todos los derechos reservados.
