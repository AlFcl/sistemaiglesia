```mermaid
erDiagram

    PERSONA {
        string RUT
        string NOMBRE
        string SEGUNDO_NOMBRE
        string APELLIDO_PATERNO
        string APELLIDO_MATERNO
        string SEXO
        string ESTADO_CIVIL
        string NACIONALIDAD
    }

    CONTACTO {
        string CONTACTO_ID
        string RUT_PERSONA
        string NUMERO_TELEFONICO
        string CORREO
    }

    DIRECCION_PERSONA {
        string ID_DIRECCION_PERSONA
        string RUT_PERSONA
        string CALLE
        string NUMERO
        string COMUNA
    }

    STAFF {
        string ID_STAFF
        string RUT_PERSONA
        string ID_AREA
        string ID_CARGO
        string NIVEL
    }

    STAFF_CARGO {
        string ID_CARGO
        string NOMBRE_CARGO
        string DESCRIPCION
    }

    STAFF_AREA {
        string ID_AREA
        string NOMBRE_AREA
        string DESCRIPCION
    }

    MUSICOS {
        string ID_MUSICO
        string RUT_PERSONA
        string INSTRUMENTO
        string ESTADO
    }

    NIVELES {
        string NIVEL
        string DESCRIPCION_NIVEL
        string ESTADO
    }

    BAUTIZO {
        string ID_BAUTIZO
        string RUT_PERSONA
        string ID_IGLESIA
    }

    IGLESIA {
        string ID_IGLESIA
        string NOMBRE_IGLESIA
        string ID_PASTORES
    }

    DIRECCION_IGLESIA {
        string ID_DIRECCION_IGLESIA
        string RUT_IGLESIA
        string CALLE
        string NUMERO
        string COMUNA
    }

    PASTORES {
        string ID_PASTORES
        string RUT_PERSONA
    }

    ESCUELA_DOMINICAL {
        string ID_ESCUELA_DOMINICAL
        string ID_IGLESIA
    }

    CURSO_DOMINICAL {
        string ID_CURSO_DOMINICAL
        string ID_IGLESIA
    }

    ALUMNO_DOMINICAL {
        string ID_ESCUELA_DOMINICAL
        string ID_IGLESIA
        string RUT_PERSONA
        string FECHA_INICIO
    }

    DICIPULADO {
        string ID_DICIPULADO
        string ID_IGLESIA
        string ID_STAFF
    }

    ALUMNO_DICIPULADO {
        string ID_ESCUELA_DOMINICAL
        string ID_IGLESIA
        string RUT_PERSONA
        string FECHA_INICIO
        string FECHA_FIN
    }

    PERSONA ||--o{ CONTACTO : tiene
    PERSONA ||--o{ DIRECCION_PERSONA : reside_en
    PERSONA ||--o{ STAFF : pertenece_a
    STAFF ||--o{ STAFF_CARGO : ocupa
    STAFF ||--o{ STAFF_AREA : trabaja_en
    PERSONA ||--o{ MUSICOS : es
    STAFF ||--o{ NIVELES : tiene
    PERSONA ||--o{ BAUTIZO : recibe
    BAUTIZO ||--o{ IGLESIA : en
    IGLESIA ||--o{ DIRECCION_IGLESIA : ubicada_en
    IGLESIA ||--o{ PASTORES : dirigida_por
    PERSONA ||--o{ PASTORES : es
    IGLESIA ||--o{ ESCUELA_DOMINICAL : tiene
    IGLESIA ||--o{ CURSO_DOMINICAL : ofrece
    PERSONA ||--o{ ALUMNO_DOMINICAL : estudia
    DICIPULADO ||--o{ IGLESIA : se_realiza_en
    DICIPULADO ||--o{ STAFF : es_guiado_por
    PERSONA ||--o{ ALUMNO_DICIPULADO : participa
