skillpassport-aa35/
├── backend/                  # Spring Boot 3.3.4 (Java 21) REST API
│   ├── src/main/java/com/skillpassport/
│   │   ├── common/           # ApiResponse, ErrorResponse, GlobalExceptionHandler
│   │   ├── config/           # OpenAPI 3, CORS, App configuration
│   │   ├── security/         # Spring Security, Password Encoder, Filter Chain
│   │   └── system/           # Diagnostic health & ping APIs
│   ├── src/main/resources/
│   │   ├── application.yml   # Base application configuration
│   │   ├── application-dev.yml # PostgreSQL & Flyway config
│   │   ├── application-local.yml # H2-Postgres fallback profile
│   │   └── db/migration/     # Versioned Flyway SQL migrations
│   └── pom.xml               # Maven dependencies (JPA, Security, JWT, PDFBox, POI)
│
├── frontend/                 # React 18 + Vite + Tailwind CSS
│   ├── src/
│   │   ├── api/              # Axios client with JWT interceptor & system service
│   │   ├── components/layout/# Navbar (with live backend status) & Footer
│   │   ├── pages/            # LandingPage & Module Views
│   │   ├── App.jsx           # React Router DOM configuration
│   │   └── main.jsx          # Entry point
│   ├── package.json
│   └── vite.config.js        # Port 5173 with backend proxy to 8080
│
├── docs/                     # Architecture documentation & diagrams
└── README.md                 # Project guide & instructions
