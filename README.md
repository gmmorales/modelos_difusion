# Unidad 015 — Modelos de difusión: leerlos, usarlos y desconfiar con criterio

**Materiales desarrollados por Matías Barreto, 2026**

**Tecnicatura Superior en Ciencias de Datos e Inteligencia Artificial — IFTS N.º 24**
* **Nomenclatura oficial:** Procesamiento Digital de Imágenes
* **Nombre de trabajo:** Laboratorio de Tecnologías de la Imagen Digital

---

Un modelo de difusión aprende a quitar ruido y, por eso, puede **inventar** lo que no está. La unidad enseña a leer y manejar estos modelos, y a distinguir en una imagen restaurada qué es dato y qué es suposición. Prepara el **Trabajo Integrador N.º 2**.

## Recorrido

| Cuaderno | Qué aprendés | Cómo se trabaja |
|---|---|---|
| [01 — La idea de la difusión](01_idea_de_la_difusion.ipynb) | Agregar y quitar ruido, y qué es `strength`. | En clase |
| [02 — Leer un modelo y generar](02_generar_y_ajustar.ipynb) | Leer la ficha de un modelo, generar y controlar `steps`, `guidance_scale` y `seed`. | En clase |
| [03 — Ampliar y limpiar](03_ampliar_y_limpiar.ipynb) | Super-resolución y reducción de ruido frente a métodos clásicos, con PSNR y SSIM. | Por tu cuenta (TPI: sub-tareas A y B) |
| [04 — Fotos antiguas](04_fotos_antiguas.ipynb) | Máscaras, inpainting clásico y con difusión, y el problema del color. | Por tu cuenta (TPI: sub-tarea C) |
| [05 — Verificar lo reconstruido](05_verificar_lo_reconstruido.ipynb) | Mapa de diferencias, SigLIP y RT-DETR; qué se puede y qué no se puede comprobar. | Por tu cuenta (TPI: análisis visual) |

Las imágenes de ejemplo están en [datos/](datos/LEEME.md), con sus fuentes y criterios de elección.

## Preparación

Todo corre en Google Colab; mirá [ANTES_DE_LA_CLASE.md](ANTES_DE_LA_CLASE.md). Los cuadernos 02 a 05 necesitan una GPU T4.

## Qué queda fuera

La edición por instrucciones con modelos grandes (FLUX.1 Kontext, Qwen-Image-Edit) no entra en la T4 gratuita sin cuantizar. Si querés usarlos para el TPI, tenés que buscar la versión cuantizada y documentar el hardware.
