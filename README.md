# ValePay

Sitio de presentación de **ValePay**: emisión de vales de despensa electrónicos
para empresas formales en México, red de comercios afiliados sin hardware, y
scoring alternativo de crédito a partir de datos transaccionales propios.

## Contenido

- `index.html` — sitio completo, autocontenido. Sin build, sin dependencias,
  sin recursos externos. Se abre con doble clic o se sirve como archivo estático.

## Modelo financiero

La proyección se construye desde una sola constante de unit economics
definida en la sección *Estructura de margen*:

| Concepto | Por cada $100 de vale emitido |
|---|---|
| Markup cobrado a la empresa | +$4.30 |
| Descuento liquidado al comercio | −$1.00 |
| Procesamiento, switch y settlement | −$1.00 |
| Fraude y fondeo del float | −$0.25 |
| × redención y share de red (60%) | × 0.60 |
| **Contribución neta** | **$4.29 (4.29%)** |

Todas las cifras de la proyección de cinco años se derivan de esa tabla.
Punto de equilibrio: **$910 MDP de volumen emitido anual · 60,700 portadores
activos · 6,300 comercios afiliados · año 4**. Requirement de capital hasta el
equilibrio: **$130 MDP** ($71 MDP de capital de trabajo + $58 MDP de pérdidas
operativas netas acumuladas).

## Aviso

Las proyecciones son estimaciones internas construidas sobre supuestos
explícitos, no hechos verificables. Este documento no constituye asesoría legal
ni financiera. Los requisitos regulatorios, fiscales y de autorización deben
validarse con un despacho especializado antes de cualquier operación.

## Publicación

```bash
git push origin main
```

GitHub Pages publica la rama `main` desde la raíz del repositorio.
