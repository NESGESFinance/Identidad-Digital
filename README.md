//
NESGES Digital Identity System

Repositorio oficial del sistema de identidad digital descentralizada del ecosistema NESGESFinance

---

Descripción General

Este repositorio contiene la arquitectura, implementación y verificación del sistema de identidad digital del ecosistema NESGESFinance Ecosystem S.A.S., desarrollado por:

Joan Santiago Ramírez Almeida
Creador, Desarrollador y CEO

El sistema está diseñado bajo un modelo criptográfico basado en la red de Bitcoin, permitiendo:

- ✔ Verificación pública de identidad
- ✔ Integridad documental mediante SHA-256
- ✔ Firma criptográfica soberana
- ✔ Anclaje inmutable en blockchain
- ✔ Auditoría descentralizada

---

Arquitectura del Sistema

El sistema se basa en un modelo de múltiples capas de verificación:

Documento Legal
      ↓
Hash SHA-256
      ↓
Firma Bitcoin (clave privada)
      ↓
Inscripción en Blockchain (TXID)
      ↓
Verificación pública

---

Estructura del JSON de Identidad

El archivo principal "identity_proof.json" contiene:

{
  "digital_identity_system": {
    "entity": "NESGESFinance Ecosystem S.A.S.",
    "controller": "Joan Santiago Ramírez Almeida",
    "layer_1_legal_document": {},
    "layer_2_signature_identity": {},
    "on_chain_registration": {},
    "bitcoin_identity": {}
  }
}

---

Componentes Clave

1. Documento Legal

- Hash SHA-256 del documento oficial
- Firma criptográfica verificada

---

2. Firma Digital (QR)

- Hash SHA-256 del archivo de firma
- Firma directa del hash
- Anclaje en blockchain mediante TXID
- Firma del TXID

---

3. Identidad Bitcoin

Dirección de firma:

1DazV8YcV6mN31So8k1ZqAxYJsSPsRWpY7

Método:

bitcoin-cli signmessage
bitcoin-cli verifymessage

---

Registro en Blockchain

El sistema ha sido anclado en la red de Bitcoin mediante una inscripción tipo Ordinal.

TXID de Registro

94cdaa726ab87513dfecee82eb00cbcf63505d38e9d55aa91d10b7acc03f40af

---

Verificación

Verificación de firma

bitcoin-cli verifymessage "1DazV8..." "FIRMA" "MENSAJE"

---

Verificación de transacción

Puede validarse públicamente mediante exploradores como:

- mempool.space
- blockstream.info

---

Verificador Web

El repositorio incluye un sistema de verificación en tiempo real compuesto por:

- Backend (Python)
- Frontend (HTML/JS)

Ejecutar backend

python server.py

---

Ejecutar frontend

python -m http.server 8000

---

Acceso

- Github: "https://raw.githubusercontent.com/NESGESFinance/Identidad-Digital/main/Authorized_Digital_Signature_QR.jpg" 
- API: "http://localhost:8080/verify"
- Web: "http://localhost:8000"

---

Integración con RWA

Este sistema forma parte del modelo de tokenización del ecosistema NESGES:

- Activos del mundo real (RWA)
- NFTs (Ordinales)
- Tokens (Runas)
- Gobernanza descentralizada

El JSON de identidad actúa como:

«Raíz de confianza criptográfica del ecosistema»

---

Propiedades del Sistema

Propiedad| Descripción
Integridad| Garantizada por SHA-256
Autenticidad| Firmas Bitcoin
Inmutabilidad| Blockchain
Transparencia| Verificación pública
No repudio| Criptografía asimétrica

---

Casos de Uso

- Identidad corporativa descentralizada
- Notarización digital
- Tokenización de activos (RWA)
- Verificación de documentos legales
- Auditoría blockchain

---

Seguridad

- No se almacenan claves privadas
- Todas las verificaciones son públicas
- Basado en criptografía estándar de Bitcoin

---

Estándar Propuesto

NESGES-DID-BTC-01

Modelo propietario de identidad descentralizada basado en:

- SHA-256
- Firmas Bitcoin
- Inscripciones Ordinales

---

Licencia

MIT License

---

Contribuciones

Este repositorio es parte del ecosistema NESGESFinance.

Para colaboraciones o integraciones institucionales:

📧 info.nesgesfinance@gmail.com

---

Ecosistema

- NESGESFinance Ecosystem
- JSRAInmob
- Tokenización RWA
- Infraestructura Blockchain

---

Conclusión

Este repositorio representa una implementación real de:

«Identidad digital descentralizada basada en Bitcoin»

con capacidad de:

- Verificación global
- Integración institucional
- Escalabilidad tecnológica

---

“Don’t trust, verify.”
