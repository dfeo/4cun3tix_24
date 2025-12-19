# Acunetix Docker

Este proyecto despliega un contenedor de Acunetix utilizando Docker Compose.

## Requisitos

- Docker
- Docker Compose

## Configuración

El servicio utiliza la imagen `daniel8812/acunetix:24`.
Por defecto, el servicio se expone en el puerto `3443`. Puedes cambiar esto configurando la variable de entorno `AWVS_PORT`.

## Uso Rápido

Para iniciar el servicio:

```bash
export AWVS_PORT=8443
docker-compose up -d
```

## Comandos útiles

```bash
# Ver logs
docker-compose logs -f

# Detener
docker-compose down

# Reiniciar
docker-compose restart

# Ver estado
docker-compose ps
```

## Acceso

Una vez iniciado, puedes acceder a la interfaz web en:
`https://localhost:8443` (o el puerto que hayas configurado).