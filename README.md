# 🍃 Rueda de Sabores del Café Interactiva

Una visualización interactiva y multilenguaje de la rueda de sabores del café, desarrollada con D3.js y diseñada para ser accesible y responsive.

![Coffee Flavor Wheel](https://img.shields.io/badge/Visualización-Interactiva-blue) ![D3.js](https://img.shields.io/badge/D3.js-v7-green) ![Multilenguaje](https://img.shields.io/badge/Idiomas-ES%20%7C%20EN-orange)

## ✨ Características

- 🎯 **Interactiva**: Haz clic en los arcos para ver detalles, doble clic para zoom
- 🌍 **Multilenguaje**: Soporte completo para español e inglés
- 🔍 **Búsqueda**: Busca descriptores específicos en tiempo real
- ♿ **Accesible**: Compatible con lectores de pantalla y navegación por teclado
- 📱 **Responsive**: Se adapta a diferentes tamaños de pantalla
- 🎨 **Diseño moderno**: Interfaz oscura y elegante

## 🚀 Demo en Vivo

**[Ver la visualización en GitHub Pages](https://tu-usuario.github.io/rueda-cafe)**

## 🛠️ Tecnologías

- **HTML5** - Estructura semántica
- **CSS3** - Diseño responsive y variables CSS
- **JavaScript ES6+** - Lógica de la aplicación
- **D3.js v7** - Visualización de datos y gráficos
- **JSON** - Datos estructurados por idioma

## 📁 Estructura del Proyecto

```
rueda-cafe/
├── index.html              # Aplicación principal
├── README.md              # Este archivo
├── .gitignore             # Archivos a ignorar en Git
└── i18n/                  # Archivos de internacionalización
    ├── es/                # Español
    │   ├── ui.json        # Textos de interfaz
    │   └── flavors.json   # Datos de sabores
    └── en/                # Inglés
        ├── ui.json        # Textos de interfaz
        └── flavors.json   # Datos de sabores
```

## 🎮 Cómo Usar

1. **Navegación**: Usa el mouse o el teclado para interactuar
2. **Selección**: Haz clic en cualquier arco para ver su información
3. **Zoom**: Doble clic en un arco para centrarlo y hacer zoom
4. **Búsqueda**: Escribe en el campo de búsqueda para encontrar descriptores
5. **Idioma**: Cambia entre español e inglés con el selector

### ⌨️ Atajos de Teclado

- `Tab` - Navegar entre elementos
- `Enter` - Activar elemento seleccionado
- `Esc` - Salir del foco del SVG

## 📊 Datos

La visualización incluye más de 50 descriptores de sabor organizados en categorías:

- **Aromas dulces** (azúcar, caramelo, miel, vainilla...)
- **Frutales** (cítricos, frutas rojas, tropicales...)
- **Floral/Herbal** (jazmín, rosa, lavanda...)
- **Especias** (canela, clavo, pimienta...)
- **Frutos secos/Cacao** (avellana, chocolate...)
- **Tostados** (malta, pan tostado...)
- **Verde/Vegetal** (guindilla, tomate...)
- **Fermento/Vinoso** (uva, vino...)
- **Off-notes** (ahumado, quemado...)

## 🔧 Desarrollo Local

1. Clona el repositorio:
```bash
git clone https://github.com/tu-usuario/rueda-cafe.git
cd rueda-cafe
```

2. Abre `index.html` en tu navegador o usa un servidor local:
```bash
# Con Python
python -m http.server 8000

# Con Node.js
npx serve .

# Con PHP
php -S localhost:8000
```

3. Visita `http://localhost:8000`

## 🌐 GitHub Pages

Este proyecto está configurado para desplegarse automáticamente en GitHub Pages:

1. Haz push a la rama `main`
2. GitHub Pages se actualizará automáticamente
3. Tu sitio estará disponible en `https://tu-usuario.github.io/rueda-cafe`

## 📝 Personalización

### Agregar Nuevos Idiomas

1. Crea una carpeta en `i18n/` con el código del idioma (ej: `fr/`)
2. Copia y traduce los archivos `ui.json` y `flavors.json`
3. Actualiza el selector de idiomas en `index.html`

### Modificar Datos

Edita los archivos JSON en `i18n/[idioma]/flavors.json` para:
- Agregar nuevos descriptores
- Modificar definiciones
- Cambiar colores
- Reorganizar categorías

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/nueva-caracteristica`)
3. Commit tus cambios (`git commit -m 'Agregar nueva característica'`)
4. Push a la rama (`git push origin feature/nueva-caracteristica`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 🙏 Agradecimientos

- Datos basados en la rueda de sabores oficial del café
- Inspirado en visualizaciones de D3.js
- Diseño accesible siguiendo las pautas WCAG

## 📞 Contacto

Si tienes preguntas o sugerencias, no dudes en abrir un issue en GitHub.

---

**Desarrollado con ❤️ para la comunidad del café**
