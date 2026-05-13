# app-carnicer-a-# Proyecto APP - Carnicería

## Estructura del proyecto para GitHub

```bash
Proyecto-App-Carniceria/
│
├── README.md
├── index.html
├── styles.css
├── app.js
├── Documentacion/
│   └── Mejoras_y_Roles_Proyecto_Carniceria.docx
│
├── Sprint_1/
├── Sprint_2/
├── Sprint_3/
├── Sprint_4/
└── Sprint_5/
```

---

# 1. README.md

```markdown
# Proyecto APP - Carnicería

## Descripción
Aplicación desarrollada para mejorar la experiencia de clientes en una carnicería mediante:

- Menús interactivos
- Seguimiento de pedidos
- Métodos de pago
- Facturación automática
- Integración con Google Maps

---

## Objetivos

- Mejorar acceso de clientes
- Modernizar la interfaz
- Automatizar procesos
- Facilitar seguimiento de pedidos

---

## Sprints del proyecto

### Sprint 1
- Recolección de datos
- Usuarios y contraseñas

### Sprint 2
- Imágenes y diseño visual

### Sprint 3
- Menús interactivos
- Responsive design

### Sprint 4
- Pagos y facturación

### Sprint 5
- Google Maps
- Notificaciones

---

## Tecnologías utilizadas

- HTML5
- CSS3
- JavaScript
- GitHub

---

## Integrantes del equipo

- Líder de proyecto
- Backend Developer
- Frontend Developer
- Diseñador UI/UX
- QA Tester
```

---

# 2. index.html

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>APP Carnicería</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

<header>
    <h1>APP Carnicería</h1>
    <p>Pedidos rápidos y seguimiento en tiempo real</p>
</header>

<nav>
    <ul>
        <li><a href="#inicio">Inicio</a></li>
        <li><a href="#menu">Menú</a></li>
        <li><a href="#pedidos">Pedidos</a></li>
        <li><a href="#pagos">Pagos</a></li>
        <li><a href="#contacto">Contacto</a></li>
    </ul>
</nav>

<section id="inicio">
    <h2>Bienvenido</h2>
    <p>Aplicación diseñada para facilitar pedidos y seguimiento de productos.</p>
</section>

<section id="menu">
    <h2>Menú Interactivo</h2>

    <div class="producto">
        <h3>Carne Premium</h3>
        <p>$250 MXN</p>
        <button onclick="agregarPedido()">Agregar pedido</button>
    </div>

    <div class="producto">
        <h3>Costillas</h3>
        <p>$180 MXN</p>
        <button onclick="agregarPedido()">Agregar pedido</button>
    </div>
</section>

<section id="pedidos">
    <h2>Seguimiento de pedidos</h2>
    <p id="estadoPedido">No hay pedidos realizados.</p>
</section>

<section id="pagos">
    <h2>Métodos de pago</h2>
    <ul>
        <li>Tarjeta bancaria</li>
        <li>Transferencia</li>
        <li>Pago contra entrega</li>
    </ul>
</section>

<footer>
    <p>Proyecto APP Carnicería - 2026</p>
</footer>

<script src="app.js"></script>
</body>
</html>
```

---

# 3. styles.css

```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    background-color: #8b0000;
    color: white;
    text-align: center;
    padding: 20px;
}

nav {
    background-color: #333;
}

nav ul {
    list-style: none;
    display: flex;
    justify-content: center;
    padding: 0;
    margin: 0;
}

nav ul li {
    margin: 10px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

section {
    padding: 20px;
}

.producto {
    background-color: white;
    padding: 15px;
    margin: 10px 0;
    border-radius: 10px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.2);
}

button {
    background-color: #8b0000;
    color: white;
    border: none;
    padding: 10px;
    cursor: pointer;
    border-radius: 5px;
}

button:hover {
    background-color: #b22222;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 15px;
}
```

---

# 4. app.js

```javascript
function agregarPedido() {
    document.getElementById("estadoPedido").innerHTML =
    "Pedido realizado correctamente. Estado: En preparación";

    alert("Producto agregado al pedido");
}
```

---

# 5. Comandos para subir a GitHub

```bash
git init

git add .

git commit -m "Primer avance proyecto app carnicería"

git branch -M main

git remote add origin https://github.com/TU-USUARIO/Proyecto-App-Carniceria.git

git push -u origin main
```

---

