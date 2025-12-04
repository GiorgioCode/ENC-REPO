# Cartografía Náutica Electrónica (ENC) bajo estándares IHO

---

## 01. Definiciones generales

![Ejemplo de carta ENC](IMG/01-ejemplo-ENC.png)

-   **ENC (Electronic Nautical Chart / Carta Náutica Electrónica)**  
    Base de datos vectorial georreferenciada estructurada según IHO.

-   **IHO (International Hydrographic Organization)**  
    Organización internacional que define estándares hidrográficos.

---

## 02. Tipos de cartas náuticas

### Comparación Raster vs ENC

![Comparación gráfica Raster vs ENC](IMG/02-RASTER-ENC1-COMPARACION-GRAFICA.png)

### Problemáticas del Raster

| Pixelado                                             | Solapamiento                                                  | Correcciones                                                       |
| ---------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------------ |
| ![Ejemplo pixelado](IMG/02-RASTER-ENC2-PIXELADO.png) | ![Solapamiento gráfico](IMG/02-RASTER-ENC3-SOLAPAMIENTO-.png) | ![Dificultades de corrección](IMG/02-RASTER-ENC4-CORRECCIONES.png) |

Raster es una imagen digital de una carta papel. No tiene atributos consultables y no es interactivo.

ENC por el contrario es vectorial, editable, con objetos y atributos.

---

## 03. Estándares relacionados IHO

![Diferencias entre S-52 / S-57 / S-63](IMG/03-DIFERENCIAS-S52-S57-S63.jpg)

-   **S-52** – Presentación visual ECDIS (símbolos, colores, prioridades)
-   **S-57** – Especificación de datos ENC
-   **S-63** – Encriptación y distribución para carta oficial segura
-   **S-101** (evolución futura)

---

## 04. Estructura técnica de una ENC

![Gráfico de Cells ENC](IMG/04-grafico-enc-cells-.png)

Las cartas ENC se dividen en **celdas**, cada una con un conjunto de objetos georreferenciados y atributos asociados.

---

## 05. Capas y datos dentro de una ENC

![Tipos de datos y capas](IMG/05-Tipos-datos-y-capas.png)

Una ENC contiene múltiples niveles de información:  
batimetría, boyas, líneas de costa, puertos, servicios y más.

---

## 06. Conceptos avanzados

### CCRP – Consistent Common Reference Point

![Ejemplo CCRP](IMG/06-CCRP-ejemplo.png)

Permite alinear Radar, AIS, ENC y sensores bajo un mismo punto de referencia.

---

## 07. Herramientas/Plugins relacionados

![Plugin Navico BR24 Radar](IMG/07-plugin-BR24.png)

Ejemplo de integración Radar Overlay con cartas ENC.

---

## 08. TO-DO técnico de desarrollo

-   [ ] Visualizador ENC con atributos consultables
-   [ ] Visualización multinivel por capas
-   [ ] Georreferenciación WGS84 + grilla
-   [ ] Integrar Radar Overlay + CCRP
-   [ ] API para consulta de objetos ENC
-   [ ] Integrar con SIHN para capas oficiales S-57

---

Fin del documento.
