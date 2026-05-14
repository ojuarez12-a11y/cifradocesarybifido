# 🔐 Cifrados Clásicos — Ética Profesional y Derecho Informático

Herramienta web interactiva para explorar y practicar dos métodos de cifrado clásico: **Cifrado César** y **Cifrado Bífido**. Desarrollada como proyecto para la materia de Ética Profesional y Derecho Informático.

---

## ✨ Características

- **Cifrado César** — cifra y descifra texto con desplazamiento ajustable (1–25)
- **Cifrado Bífido** — cifra y descifra usando el cuadro de Polibio 5×5
- **Paso a paso** — visualización guiada o libre del proceso de cifrado/descifrado
- **Rueda de César** — visualización animada del desplazamiento del alfabeto
- **Tabla del alfabeto** — muestra en tiempo real la correspondencia de letras
- **Cuadro de Polibio** — resalta las letras involucradas en cada operación
- **Comparativa** — análisis lado a lado de ambos métodos (complejidad, seguridad, uso histórico)
- **Modo Presentación** — pantalla completa para exponer el proyecto
- **Tema claro/oscuro** — alternancia con un clic
- **Diseño responsive** — funciona en móvil y escritorio

---

## 🚀 Cómo usar

No requiere instalación ni dependencias. Solo abre el archivo en un navegador:

```bash
# Opción 1 — abrir directamente
Doble clic en index.html

# Opción 2 — servidor local (opcional)
npx serve .
# o
python -m http.server 8080
```

Luego visita `http://localhost:8080` si usaste servidor local.

---

## 📂 Estructura del proyecto

```
proyecto/
└── index.html      # Aplicación completa (HTML + CSS + JS en un solo archivo)
└── README.md       # Este archivo
```

---

## 🔢 Métodos de cifrado

### Cifrado César

Sustitución monoalfabética que desplaza cada letra del mensaje un número fijo de posiciones en el alfabeto.

- **Fórmula cifrado:** `C = (P + K) mod 26`
- **Fórmula descifrado:** `P = (C − K + 26) mod 26`
- **Clave:** valor de desplazamiento K (1–25)
- **Ejemplo con K=3:** `HOLA` → `KROD`

### Cifrado Bífido

Cifrado polibiano que combina sustitución y transposición usando un cuadro 5×5.

- Utiliza el **Cuadro de Polibio** con el alfabeto de 25 letras (I/J comparten celda)
- **Cifrado:** convierte letras a coordenadas → separa filas y columnas → recombina → nuevas letras
- **Descifrado:** proceso inverso
- **Nota:** La Ñ y la J no forman parte del alfabeto del cuadro (J se trata como I)

---

## 🛠️ Tecnologías

| Tecnología | Uso |
|---|---|
| HTML5 | Estructura |
| CSS3 | Estilos, animaciones, tema oscuro/claro |
| JavaScript (vanilla) | Lógica de cifrado, UI dinámica |
| Google Fonts | Tipografías IBM Plex Mono y Syne |

---

## 📖 Notas académicas

- Este proyecto es de carácter **educativo**; los cifrados César y Bífido son métodos históricos considerados inseguros para uso real.
- El Cifrado César fue utilizado por Julio César para comunicaciones militares (~50 a.C.).
- El Cifrado Bífido fue inventado por Félix Delastelle en 1901 y combina dos técnicas criptográficas: sustitución y transposición.

---

## 👤 Autor

Universidad Autonoma de Baja California Sur
Departamento Academico de Sistemas Computacionales
II Semestre - Ingeniería en Desarrollo de Software

Proyecto académico — Materia: Ética Profesional y Derecho Informático  
Alumnos:    Oswaldo Juarez Jimenez
            Sergio Angel Rochin Rodriguez
