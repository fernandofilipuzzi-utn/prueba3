# Diagrama de clases - UML

### Diagrama de flujo de autenticación

```mermaid
flowchart TD
    A[Usuario] -->|Inicia sesión| B[Frontend]
    B --> C[API Backend]
    C --> D{¿Credenciales válidas?}
    D -- Sí --> E[Generar Token JWT]
    D -- No --> F[Mostrar error]
    E --> G[Frontend recibe token]
    G --> H[Accede a recursos]
