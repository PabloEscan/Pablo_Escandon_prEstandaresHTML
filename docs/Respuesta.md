# Respuesta a la auditoria recibida

**Encargado de la revisión:** Jefferson Xavier Guerrero Sisalima

**Nº:** 12

---

## Tabla de respuesta:

| N. | Decisión (acepta o refuta) | Justificación con la norma | Evidencia antes y después | Commit |
| :---: | :--- | :--- | :--- | :--- |
| 1 | Aceptada | El contraste que se producia entre el botón y texto era insuficiente apenas de un 3.67:1, la norma tiene como mínimo un 4,5:1. | La evidencia esta adjunta en cuatro imagenes. El primer par muestra el contraste antes y despúes en la web son aquelas que cuentan `con _web` , mientras que el otro par muestran el contraste con el color anterior y el nuevo usando WebAIM Contrast Checker. |  Segundo commit que incluira la corrección de colores, unificando varios colores parecidos, los resultados se veran ilustrados en el root del archivo CSS. |
| 2 | Aceptada | Los campos de nombre, correo y teléfono deben tener el atributo `autocomplete` para que los navegadores puedan rellenar automáticamente estos campos con los datos guardados del usuario. | La evidencia se encuentra en la captura `autocompletadoAgregado`, donde se comprueba en el DOM que los atributos `autocomplete` (name, email y tel) fueron añadidos correctamente a los tres campos del formulario.| Se realizara en el segundo commit, junto a las evidencias respectivas.  |
| 3 | Aceptada | Como bien se menciona en la auditoría recibida, no se tiene un control sobre el estado `min/max` en el apartado de fecha en el registro. | La evidencia está dividida en dos capturas del código HTML antes y después del input con el id `min/max`. | El commit será realizado como el primero para agregar la auditoría recibida y junto a la primera parte de la respuesta. |
| 4 | Aceptada | El campo de imagen si tiene mero proposito decorativo no debe tener nara entre el `alt`, por ende se debe eliminar el texto que estaba entre estos corchetes quedando unicamente `alt=""` | La evidencia esta en el DOM que se puede inspeccionar en la página web o revisar el código directamente. | El commit será el sergundo junto a las otras dos revisiones, concluyendo el apartado tres su no se encuentran errores propios |

## Tabla de errores propios

| N.º | Justificación con la norma | Evidencia antes y después | Commit |
| :---: | :--- | :--- | :--- |
| 1 | Un error en la línea 11 del código esta escrito "calss", pese a no usar ningun IDs, es mejor limpiar el código para evitar errores de sintaxis en el validador W3C | La evidencia se puede observar por el DOM. |  Segundo commit junto al resto de correcciones de la respuesta. |
| 2 | WCAG 2.2, criterio 1.4.10 (Reflow) y especificación W3C CSS Grid, el contenido debe adaptarse a un viewport, en este caso el breakpoint es de 768 px. El contenido de <aside> no seguía esta norma, este se desplegaba| La evidencia se  encuentra en una imagen llamada `PruebaAside768Antes` el cambio se verá reflejado en la página web. |  Segundo commit junto al resto de correcciones de la respuesta. |