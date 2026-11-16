# Redes y Comunicaciones IP · Actividad práctica Capa 7

Sitio web académico en HTML para la asignatura **INTERNET: Redes y Comunicaciones IP**, con el resumen de lo aprendido en los cursos de Cisco Networking Academy y en los laboratorios de GNS3. Se publica con nginx dentro de un contenedor Docker para poder replicarlo en cualquier máquina.

## Páginas

| Página | Contenido |
|---|---|
| `index.html` | Inicio y presentación del sitio |
| `html-puro.html` | Lo aprendido en el curso, solo con etiquetas HTML |
| `html-css.html` | El mismo contenido con la hoja de estilos `css/estilos.css` |
| `integrantes/camilo.html` | Breve biografía de Camilo Novoa Montenegro |

## Estructura

```text
.
├── README.md
├── Dockerfile
├── docker-compose.yml
├── index.html
├── html-puro.html
├── html-css.html
├── css/
│   └── estilos.css
├── img/
│   └── topologia.svg
└── integrantes/
    └── camilo.html
```

## Requisitos

- Docker Desktop (Windows/macOS) o Docker Engine (Linux)

## Ejecución con Docker Compose

```bash
docker compose up -d --build
```

Abrir en el navegador: <http://localhost:8002>

Detener el servicio:

```bash
docker compose down
```

## Ejecución solo con Docker

```bash
docker build -t sitio-camilo .
docker run -d -p 8002:80 --name sitio-camilo sitio-camilo
```

## Integrante

- Camilo Novoa Montenegro · Universidad de Ibagué

## Licencia

Uso académico.
