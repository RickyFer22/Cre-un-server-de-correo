# Configuración de Poste.io con Docker Compose

Este repositorio contiene una configuración sencilla de Poste.io usando Docker Compose.  Permite configurar un servidor de correo electrónico rápidamente.

## Requisitos

* Docker
* Docker Compose
* Una cuenta en GitHub

## Uso

1. **Clona el repositorio:**
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   cd <NOMBRE_DEL_REPOSITORIO>
   ```

2. **Crea el directorio de datos:**
   ```bash
   mkdir mail-data
   ```

3. **Personaliza el archivo `docker-compose.yml`:**
   * Cambia `POSTE_IO_DOMAIN` a tu propio dominio.  Ejemplo: `POSTE_IO_DOMAIN=tudominio.com`
   * Cambia `POSTE_IO_HOSTNAME` a tu propio hostname. Ejemplo: `POSTE_IO_HOSTNAME=mail.tudominio.com`

4. **Inicia Poste.io:**
   ```bash
   docker-compose up -d
   ```

5. **Accede a la interfaz de administración:**  Abre tu navegador web en `https://mail.tudominio.com` (reemplazando `tudominio.com` con tu dominio).

6. **Para subir los cambios a GitHub:**
    ```bash
    git add .
    git commit -m "Initial commit"
    git push origin main  
    ```
    (Reemplaza `main` con el nombre de tu rama principal si es diferente)


## Documentación adicional

* [Documentación oficial de Poste.io](https://poste.io/doc/)
* [Video tutorial (opcional)](https://www.youtube.com/watch?v=K4-uD1VHCz0)


## Consideraciones

* Asegúrate de tener un dominio configurado correctamente con registros DNS (MX, A, etc.) apuntando a tu servidor.
* Este es un ejemplo básico.  Para configuraciones más avanzadas, consulta la documentación de Poste.io.
