Mercado Libre · Mock Producto 3D/AR (Demo en vivo)

Qué es
------
Una página simple que simula una ficha de producto de Mercado Libre con un botón "Ver en 3D"
que despliega un visor 3D y permite abrir AR nativo (Scene Viewer en Android, Quick Look en iOS).

Cómo usarla (en 3 minutos)
--------------------------
1) Publicá esta carpeta:
   - Opción rápida: https://app.netlify.com/drop → arrastrá el ZIP y obtené una URL.
   - Alternativa: GitHub Pages (subí como repo y activá Pages).

2) Abrí la URL desde tu celular. Tocá "👓 Ver en 3D" y luego "Ver en tu espacio (AR)".
   - iOS abrirá Quick Look (USDZ).
   - Android abrirá Scene Viewer (GLB).

3) Compartí un QR con la URL para que todos la prueben desde sus teléfonos.

Cómo reemplazar el modelo por una Zapatilla
-------------------------------------------
- En index.html cambiá:
  src="https://modelviewer.dev/shared-assets/models/Astronaut.glb"
  ios-src="https://modelviewer.dev/shared-assets/models/Astronaut.usdz#allowsContentScaling=1"
  por las rutas a tu GLB y USDZ (ideal ≤ 2–5 MB, escala en metros).
- Sugerencia: asegurate de que el modelo esté a escala real para que AR se vea creíble sobre una mesa.

Plan B si AR falla
------------------
- El visor 3D funciona igual (rotación/zoom).
- Llevá un video corto de respaldo mostrando AR en tu casa/escritorio por si el Wi-Fi del salón no anda.

Presentación sugerida (guion 60–90 s)
-------------------------------------
1) Mostrá la ficha normal (fotos). Dolor: “no veo tamaño real / no veo atrás / etc.”
2) Tocá “Ver en 3D” → girá el producto.
3) Tocá “Ver en tu espacio” → colocá el objeto en una mesa. Mencioná: “escala real”.
4) Cierre: “con un piloto de 150 SKUs medimos conversión y devoluciones en 6–8 semanas”.

Notas técnicas
--------------
- Este mock usa <model-viewer> (Web Component). Detecta el dispositivo y lanza el modo AR indicado.
- Formatos: GLB para Android (Scene Viewer), USDZ para iOS (Quick Look).

¡Éxitos con la demo!
