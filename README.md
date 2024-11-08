<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Sitio Web Accesible</title>
    <!-- Enlace a Bootstrap -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
    <!-- Enlace a CSS personalizado -->
    <link rel="stylesheet" href="colores.css">
    <style>
        /* CSS para transición suave */
        .carousel-item {
            transition: transform 1s ease-in-out; /* Ajusta el tiempo de transición aquí */
        }
    </style>
</head>
<body>

    <!-- Encabezado con barra de navegación -->
    <header>
        <nav class="navbar navbar-expand-lg navbar-light bg-light" aria-label="Barra de navegación">
            <div class="container-fluid">
                <a class="navbar-brand" href="#">Mi Sitio Web</a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Alternar navegación">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNav">
                    <ul class="navbar-nav ms-auto">
                        <li class="nav-item">
                            <a class="nav-link active" href="#inicio" aria-current="page">Inicio</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#productos">Productos</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#contacto">Contacto</a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </header>

    <!-- Sección de bienvenida -->
    <section id="inicio" class="bg-primary text-white text-center p-5">
        <div class="container">
            <h1>¡Bienvenidos a Mi Sitio Web!</h1>
            <p class="lead">Aquí encontrarás productos exclusivos con las mejores tendencias.</p>
        </div>
    </section>

    <!-- Sección de productos destacados -->
    <section id="productos" class="py-5">
        <div class="container">
            <h2 class="text-center">Productos Destacados</h2>
            <!-- Carrusel con transición -->
            <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel" data-bs-interval="3000">
                <div class="carousel-indicators">
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="3" aria-label="Slide 4"></button>
                    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="4" aria-label="Slide 5"></button>
                </div>
                <div class="carousel-inner">
                    <div class="carousel-item active">
                        <img src="producto1.jpg" class="d-block w-100" alt="Descripción del Producto 1">
                        <div class="carousel-caption d-none d-md-block">
                            <h5>Producto 1</h5>
                            <p>$29.99</p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="producto2.jpg" class="d-block w-100" alt="Descripción del Producto 2">
                        <div class="carousel-caption d-none d-md-block">
                            <h5>Producto 2</h5>
                            <p>$39.99</p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="producto3.jpg" class="d-block w-100" alt="Descripción del Producto 3">
                        <div class="carousel-caption d-none d-md-block">
                            <h5>Producto 3</h5>
                            <p>$49.99</p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="producto4.jpg" class="d-block w-100" alt="Descripción del Producto 4">
                        <div class="carousel-caption d-none d-md-block">
                            <h5>Producto 4</h5>
                            <p>Descripción del producto 4.</p>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <img src="producto5.jpg" class="d-block w-100" alt="Descripción del Producto 5">
                        <div class="carousel-caption d-none d-md-block">
                            <h5>Producto 5</h5>
                            <p>Descripción del producto 5.</p>
                        </div>
                    </div>
                </div>
                <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Previous</span>
                </button>
                <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Next</span>
                </button>
            </div>
        </div>
    </section>

    <!-- Sección de contacto -->
    <section id="contacto" class="bg-light py-5">
        <div class="container">
            <h2 class="text-center">Contacto</h2>
            <form action="#" method="post" aria-label="Formulario de contacto">
                <div class="mb-3">
                    <label for="nombre" class="form-label">Nombre:</label>
                    <input type="text" id="nombre" name="nombre" class="form-control" aria-required="true">
                </div>
                <div class="mb-3">
                    <label for="email" class="form-label">Correo Electrónico:</label>
                    <input type="email" id="email" name="email" class="form-control" aria-required="true">
                </div>
                <div class="mb-3">
                    <label for="mensaje" class="form-label">Mensaje:</label>
                    <textarea id="mensaje" name="mensaje" rows="5" class="form-control" aria-required="true"></textarea>
                </div>
                <div class="text-center">
                    <button type="submit" class="btn btn-primary">Enviar</button>
                </div>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark text-white text-center p-3">
        <p>&copy; 2024 Mi Sitio Web - Todos los derechos reservados.</p>
    </footer>

    <!-- Enlace a Bootstrap JS (necesario para el funcionamiento del navbar) -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
