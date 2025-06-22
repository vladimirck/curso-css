# Exploración de Controles de Formularios en HTML

## Datos del participante

- **Nombre**: Domingo V Pérez
- **Código**: 990642
- **Escuela**: Escuela de Física

## Objetivos de la práctica

- Reconocer y comprender los tipos de controles más comunes en formularios HTML5.
- Aplicar correctamente las etiquetas `<input>` en sus diferentes variantes.
- Visualizar en el navegador el comportamiento de cada tipo de campo.
- Diferenciar entre tipos de datos que se pueden capturar con cada control.

## Desarrollo

Para cumplir con las instrucciones de la tarea, creé un archivo llamado `formulario.html`. Transcribí manualmente el código proporcionado para comprender el funcionamiento de cada control. Al finalizar, instalé la extensión Prettier en Visual Studio Code para asegurar un formato de código consistente y profesional, superior al que se logra manualmente.

El resultado final del documento, una vez transcrito y formateado, es el siguiente:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>

  <body>
    <form action="">
      <p>
        Selección de un color <br />
        <input type="color" name="" value="" />
      </p>
      <p>
        Fecha <br />
        <input type="date" name="" value="" />
      </p>
      <p>
        Fecha y hora <br />
        <input type="datetime" name="" value="" />
      </p>
      <p>
        Archivo plano, archivo de Word, Excel ... <br />
        <input type="file" name="" value="" />
      </p>
      <p>
        Email <br />
        <input type="email" name="" value="" />
      </p>
      <p>
        Mes <br />
        <input type="month" name="" value="" />
      </p>
      <p>
        Número <br />
        <input type="number" name="" value="" />
      </p>
      <p>
        Rango de número<br />
        <input type="range" min="0" max="10" name="" value="" />
      </p>
      <p>
        Búsqueda<br />
        <input type="search" name="" value="" />
      </p>
      <p>
        Teléfono<br />
        <input type="tel" name="" value="" />
      </p>
      <p>
        Hora <br />
        <input type="time" name="" value="" />
      </p>
      <p>
        Dirección URL <br />
        <input type="url" name="" value="" />
      </p>
      <p>Semana <br /><input type="week" name="" value="" /></p>
      <p>Reset<br /><input type="reset" name="" value="Reset" /></p>
      <p>
        Botón HTML <br />
        <input type="button" name="" value="Botón HTML" />
      </p>
      <p>
        Envío de formulario<br /><input type="submit" name="" value="Enviar" />
      </p>
    </form>
  </body>
</html>
```

## Reflexión sobre la Aplicabilidad de los Controles de Formulario

Cada tipo de control de formulario en HTML5 ofrece funcionalidades específicas que son valiosas en distintos contextos. A continuación, se analiza la utilidad de cada elemento probado, con un enfoque en su aplicación en el entorno académico.

**1. Selector de Color (`type="color"`)**
Este control es ideal para permitir la personalización de elementos visuales, como el color de fuentes o gráficos en una aplicación. Su interfaz intuitiva facilita la selección. Sin embargo, debido a la alta granularidad (la gran cantidad de colores disponibles), podría ser más adecuado para una sección de "configuración avanzada". Para un uso más general, sería preferible ofrecer una paleta de colores predefinidos para simplificar la elección del usuario.

**2. Entradas de Fecha y Hora (`date`, `datetime`, `time`, `week`, `month`)**
Estos campos son fundamentales en el ámbito académico para definir plazos, cronogramas y horarios.

- **Observación de Usabilidad:** Noté que el campo de fecha (`date`) despliega un calendario contextual muy útil. Sin embargo, el campo de fecha y hora (`datetime`) no mostró una interfaz similar en los navegadores probados, lo que dificulta su uso. Para una mejor experiencia de usuario, es más efectivo separar la captura de datos en dos campos: uno para la fecha (`date`) y otro para la hora (`time`). También es posible utilizar `datetime-local`, que noté que sí es soportado por el browser.
- **Granularidad:** Los campos para mes (`month`) y semana (`week`) son perfectos para planificaciones de alto nivel, como cronogramas de asignaturas semestrales o planes de estudio mensuales, donde no es necesario especificar un día exacto.

**3. Selector de Archivos (`type="file"`)**
La capacidad de adjuntar y enviar archivos es esencial en un entorno educativo para la entrega de tareas, proyectos e informes. Una mejora importante para su implementación práctica sería utilizar el atributo `accept` para limitar los tipos de archivo permitidos (ej. `.pdf`, `.docx`), asegurando que solo se reciban los formatos correctos.

**4. Campos de Contacto (`email`, `tel`)**
Los campos de correo electrónico y teléfono son cruciales para los formularios de registro o contacto, ya que facilitan la comunicación inicial y continua entre docentes, estudiantes y personal administrativo. El navegador además valida automáticamente que el formato del email sea el correcto.

**5. Campos Numéricos (`number`, `range`)**
Estos controles son muy versátiles para tareas académicas cuantitativas, desde la recolección de datos en encuestas hasta la creación de cuestionarios en materias como matemáticas o física. El tipo `range` es particularmente útil, ya que restringe la entrada de datos a un rango válido, minimizando errores de captura.

**6. Campo de Búsqueda (`type="search"`)**
Este campo mejora la experiencia del usuario en sitios con gran cantidad de contenido, como portales de investigación o bibliotecas digitales. Permite a los usuarios encontrar información específica de manera rápida y eficiente.

**7. Campo de URL (`type="url"`)**
Muy útil para que los estudiantes compartan recursos o proyectos alojados en plataformas externas. Por ejemplo, pueden enviar enlaces a sus repositorios en GitHub, a cuadernos de Google Colab, o a artículos de investigación y otras fuentes científicas en línea.

**8. Botones (`submit`, `reset`, `button`)**
Estos tres elementos, aunque visualmente similares, tienen propósitos distintos y fundamentales:

- **`type="submit"` (Enviar):** Indica al usuario que ha completado el formulario y desea enviar los datos al servidor.
- **`type="reset"` (Restablecer):** Permite al usuario borrar toda la información introducida y devolver el formulario a su estado inicial.
- **`type="button"` (Botón genérico):** Es un botón sin acción predeterminada. Es ideal para ejecutar funciones personalizadas a través de JavaScript, como mostrar/ocultar elementos, realizar cálculos en una calculadora virtual o activar otras interacciones en la interfaz.

En conclusión, el dominio de estos controles es esencial para desarrollar páginas web y aplicaciones académicas que sean funcionales, interactivas y fáciles de usar, tanto en aplicaciones de carácter general, como en aplicaciones académicas.
