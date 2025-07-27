flowchart TD
    A[Presentación de Roles del Proyecto]

    subgraph Equipo de estudio
        A1[Marcelo Flores QA]
        A2[Piero Zamora FrontEnd]
        A3[Gabriel Coaguila BackEnd]
        A4[Barbara Cuba Android]
        A5[Alejandro Mendoza Android]
        A6[Deyci Camargo Android]
        A7[Vanessa Condori FrontEnd]
        A8[Aleyda Quispe FrontEnd]
        A9[Jose Kana Backend]
    end

    subgraph Herramientas
        G[Git Sistema de control de versiones]
        H[GitHub Colaboración en la nube]
    end

    subgraph Roles Técnicos
        R1[Frontend UI, interactividad, APIs]
        R2[Backend Lógica, BD, APIs]
        R3[Android Apps móviles con Kotlin/Java]
        R4[QA Pruebas y calidad]
    end

    A --> Equipo_de_estudio
    Equipo_de_estudio --> G
    Equipo_de_estudio --> H
    G --> H

    A2 --> R1
    A7 --> R1
    A8 --> R1

    A3 --> R2

    A4 --> R3
    A5 --> R3
    A6 --> R3

    A1 --> R4

    R1 -->|Interfaz| R2
    R2 -->|Datos/API| R1
    R3 -->|Requiere lógica y API| R2
    R4 -->|Testea| R1
    R4 -->|Testea| R2
    R4 -->|Testea| R3

    H -->|Control y versión de código| Roles_Técnicos
