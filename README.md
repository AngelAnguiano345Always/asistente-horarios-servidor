# Asistente Inteligente de Horarios Universitarios

Proyecto academico para la materia de Programacion Logica y Funcional.

## Descripcion

Sistema web que recibe informacion del estudiante (materias, horas de sueno, estres, tiempo libre) y genera recomendaciones personalizadas de horarios de estudio, alertas de sobrecarga y sugerencias de descanso.

## Paradigmas implementados

| Paradigma | Herramienta de diseno | Archivo en Python |
|-----------|----------------------|-------------------|
| Logico    | Prolog (SWISH)       | `logica.py`       |
| Funcional | CLISP (JDoodle)      | `funcional.py`    |
| Imperativo / Web | Flask (Python) | `app.py`       |

## Estructura del proyecto

```
asistente-horarios-universitarios/
├── app.py              Servidor Flask principal
├── logica.py           Reglas logicas (traducidas de Prolog)
├── funcional.py        Funciones (traducidas de CLISP)
├── requirements.txt    Dependencias de Python
├── prolog/
│   └── reglas.pl       Codigo Prolog original (SWISH)
├── lisp/
│   └── funciones.lisp  Codigo CLISP original (JDoodle)
├── templates/
│   └── index.html      Interfaz web
└── static/
    ├── css/style.css   Estilos
    └── js/main.js      Interacciones
```

## Como ejecutar localmente (en Replit)

1. Abrir el proyecto en Replit
2. En la terminal ejecutar:
   ```
   pip install -r requirements.txt
   python app.py
   ```
3. Hacer clic en el boton "Open in new tab" que aparece en Replit

## Codigo Prolog (para ejecutar en SWISH)

Ir a: https://swish.swi-prolog.org  
Pegar el contenido de `prolog/reglas.pl`

Consultas de ejemplo:
```prolog
?- horas_estudio_recomendadas(alta, 5, H).
?- calidad_sueno(6.5, Calidad).
?- sobrecarga(7, muy_alta, 4, critico).
```

## Codigo CLISP (para ejecutar en JDoodle)

Ir a: https://www.jdoodle.com/execute-clisp-online  
Pegar el contenido de `lisp/funciones.lisp`  
Hacer clic en Execute.

## Integrantes

- Persona 1: Frontend (HTML, CSS, JavaScript)
- Persona 2: Backend (Flask, logica.py, funcional.py, app.py)
- Persona 3: Logica y funcional (Prolog, CLISP, documentacion)
