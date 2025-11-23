
# Sistema Didáctico de Medición Cognitiva y Emocional ...

Plataforma modular orientada a la **creación, ejecución y análisis de tests cognitivo–emocionales**, con foco en didáctica, investigación y medición perceptiva.  
Este repositorio contiene el código fuente del sistema, su documentación base y la arquitectura establecida por el equipo.

---

## 🚀 Objetivo del Proyecto
Construir una herramienta capaz de:
- Diseñar tests estructurados y dinámicos.
- Registrar respuestas de usuarios de forma anónima.
- Procesar puntajes por dimensiones cognitivas/emocionales.
- Presentar resultados en dashboards simples y exportables.
- Permitir análisis posteriores por campañas y canales.

Este proyecto también sirve como **demostrador profesional** de arquitectura, diseño de sistemas, UX y desarrollo colaborativo.

---

## 🧱 Arquitectura General
El sistema se estructura en tres capas principales:

```
Frontend (SPA)
    ↓ API JSON
Backend (REST API)
    ↓ ORM / Servicios
Base de Datos (Relacional)
```

- **Frontend**: SPA moderna (React/Vue/Svelte)  
- **Backend**: Node/NestJS o Laravel (según decisión de equipo)  
- **Base de datos**: MariaDB / MySQL  
- **ORM**: Prisma / Eloquent / TypeORM (a definir)

---

## 📂 Estructura del Repositorio (Monorepo)

```
/frontend        → Aplicación del usuario final y panel administrativo
/backend         → API, modelos, migraciones, controladores
/docs            → Documentación técnica y funcional
/scripts         → Herramientas de automatización
/.github         → Templates, CI/CD y configuraciones
```

---

## 📘 Documentación del Proyecto

Los siguientes documentos forman la base formal del sistema:

- **Proyecto_Sistema_Didactico.docx** — idea, visión y fundamentos  
- **Requerimientos_Funcionales.docx** — RF/RNF + alcances  
- **Especificación y Diagramas** — arquitectura, endpoints, backlog  
- **Convención_de_Nombres_Sistema_Didactico.docx** — diccionario de datos, naming estándar  

Toda la documentación se encuentra en la carpeta `/docs`.

---

## 🧩 Convención de Nombres (Resumen)
- **Base de datos** → `snake_case`  
- **API / Frontend / Backend** → `camelCase`  
- **Componentes frontend** → PascalCase  
- **Commits** → estándar convencional (`feat:`, `fix:`, `docs:`…)  

Más detalles en `/docs/Convencion_de_Nombres`.

---

## 🛠 Setup Inicial

### 1) Clonar repositorio
```bash
git clone https://github.com/<tu-org>/<tu-repo>.git
cd <tu-repo>
```

### 2) Instalar dependencias (cuando el stack esté definido)
Frontend:
```bash
cd frontend
npm install
```

Backend:
```bash
cd backend
npm install
```
o  
```bash
composer install
```

### 3) Variables de entorno
```
cp .env.example .env
```

Agregar credenciales de:
- BD  
- JWT / APP_KEY  
- CORS  
- Paths de frontend  

---

## 🧪 Scripts típicos

Frontend:
```bash
npm run dev
npm run build
```

Backend (Node):
```bash
npm run start:dev
npm run migrate
```

Backend (Laravel):
```bash
php artisan serve
php artisan migrate
```

---

## 🎯 Alcance del MVP (validado)
- Crear/editar tests  
- Banco de preguntas  
- Ejecución anónima  
- Registro de respuestas  
- Cálculo de dimensiones  
- Dashboard básico  
- Roles mínimos: admin / viewer  
- Exportación simple  

---

## 📅 Roadmap General

### **Sprint 0 — Preparación**
- Configurar repositorio  
- Migraciones iniciales  
- Modelos + ORM  
- Estructura frontend  
- Integración API

### **Sprint 1 — Builder + Ejecución**
- CRUD de tests  
- Preguntas + opciones  
- Ejecución del test  
- Persistencia de respuestas

### **Sprint 2 — Análisis + Dashboard**
- Cálculo de dimensiones  
- Vista administrativa  
- Exportar resultados

### **Sprint 3 — Pulido y versión pública**
- Autenticación sólida  
- Estilos y UX  
- Preparar demo  

---

## 🤝 Contribución (Flujo sugerido)

Ramas:
- `main` → producción  
- `dev` → desarrollo activo  
- `feature/<nombre>` → nuevas funciones  

Reglas:
1. Crear issue antes de desarrollar  
2. Hacer PR hacia `dev`  
3. Revisión por 1 miembro  
4. Merge y cierre de issue automáticamente  

---

## 📄 Licencia
Licencia a definir por el equipo (MIT recomendada).

---

## 👥 Equipo
- **Líder conceptual / arquitectura:** @tu-usuario  
- **Desarrollo (backend):** *a definir*  
- **Desarrollo (frontend):** *a definir*  
- **UX/creativo:** *a definir*  

---

## 🚀 Estado del Proyecto
> Documentación base completa.  
> En etapa de definición de tecnologías y setup inicial.  
> Próxima reunión: asignar roles, mockups y stack final.
