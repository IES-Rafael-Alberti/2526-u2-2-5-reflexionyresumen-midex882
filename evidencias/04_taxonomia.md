# **ENTREGA \- Investigación y Desarrollo de la Taxonomía de Incidentes de Ciberseguridad**

**ID Actividad:** 2.a.01  
**RA y CE Evaluados:** RA2, CE a  
**Formato:** Documento único en Markdown

## **Datos del Grupo**

| Campo | Contenido |
| ----- | ----- |
| **Nombres de miembros** | Jose María Escalón Prada, Abel García Domínguez, David Jimenez Ruiz, Daniel Hernández Gómez |
| **Número de miembros** | 4 |
| **URL del repositorio** | https://github.com/IES-Rafael-Alberti/2526-u2-2-1-taxonomia-grupo-3\_2526.git |
| **Rama principal** | master |
| **Fecha de entrega** | 15/01/2026 |

##  **Agrupaciones Seleccionadas**

##  **Agrupación 1: Contenido malicioso**

**Descripción:** Incidentes en los que se detecta código o contenido malicioso que afecta o se distribuye desde sistemas de la organización, incluyendo infecciones de malware, servidores de mando y control, distribución de malware y recursos que almacenan configuraciones de malware.

**Tipos documentados:** 4

## **Agrupación 2: Intento de intrusión**

**Descripción:** Incidentes en los que se observa un intento de comprometer la confidencialidad, integridad o disponibilidad de los sistemas, ya sea explotando vulnerabilidades conocidas, vulnerando credenciales o mediante ataques con exploits desconocidos o zero‑day.​

**Tipos documentados:** 4

##  **DOCUMENTACIÓN COMPLETA \- AGRUPACIÓN 1 (Contenido malicioso)**

## **Tipo 1: Sistema infectado**

## **Características**

| Campo | Contenido |
| ----- | ----- |
| **Descripción** | Incidente en el que uno o varios sistemas (PC, servidor o dispositivo móvil) resultan infectados por malware, como troyanos bancarios, rootkits o ransomware, comprometiendo su funcionamiento y la información almacenada.    |
| **Funcionamiento** | El atacante consigue que el usuario ejecute código malicioso (APK, ejecutable, script, etc.), aprovechando ingeniería social o software trojanizado.    Una vez ejecutado, el malware se instala, obtiene permisos y comienza a robar datos o comunicarse con C\&C.    |
| **Identificación** | Detecciones del antivirus/EDR, tráfico inusual hacia IPs sospechosas, consumo anómalo de recursos, aparición de aplicaciones desconocidas, cambios en permisos y generación de logs con errores o conexiones no autorizadas.    |
| **Protección** | Uso de soluciones antimalware actualizadas, políticas de instalación restringida, concienciación frente a apps no oficiales, segmentación de red, actualización de sistemas y monitorización de tráfico saliente hacia dominios maliciosos.    |

## **Caso Real**

| Parámetro | Contenido |
| ----- | ----- |
| **URL** | [https://securelist.com/it-threat-evolution-q1-2024-mobile-statistics/112750/](https://securelist.com/it-threat-evolution-q1-2024-mobile-statistics/112750/) |
| **Breve Descripción** | Kaspersky reportó que en el primer trimestre de 2024 bloqueó 10,1 millones de ataques de malware, adware o software no deseado contra dispositivos móviles Android de sus usuarios, incluyendo troyanos bancarios y ransomware móvil, lo que evidencia un volumen elevado de sistemas móviles infectados en todo el mundo.    |
| **Agrupación/Tipo** | Contenido malicioso \> Sistema infectado |
| **Origen** | Externo |
| **Perfiles Afectados** | Usuarios generales de dispositivos móviles, tanto particulares como empleados que usan móviles personales o corporativos.    |
| **Nº y Tipología Sistemas** | Millones de dispositivos móviles Android de usuarios de Kaspersky, afectados o potencialmente afectados por intentos de infección.    |
| **Categoría Sistemas** | Alta (afecta a dispositivos de usuario que pueden contener credenciales, datos personales y acceso a servicios corporativos).    |
| **Peligrosidad** | 4 |
| **Impacto** | L4 |
| **Prioridad Asignada** | Alta |

## **Tipo 2: Sistema infectado con malware (troyano bancario móvil)**

## **Características**

| Campo | Contenido |
| ----- | ----- |
| **Descripción** | En este caso un sistema resulta infectado con un malware específico, como un troyano bancario, que tiene como objetivo principal el robo de credenciales financieras y otros datos sensibles para realizar fraude económico.   |
| **Funcionamiento** | El usuario instala una app maliciosa que se hace pasar por un servicio legítimo, el malware oculta su icono, mantiene persistencia en segundo plano, intercepta SMS, captura información de banca online y abusar de certificados digitales para suplantar al usuario.    |
| **Identificación** | Instalación de aplicaciones fuera de canales oficiales, demasiados permisos, conexiones a dominios sospechosos, quejas de usuarios sobre operaciones bancarias no reconocidas y alertas del banco por acceso no identificados.    |
| **Protección** | Uso de tiendas oficiales, revisión de permisos, soluciones de seguridad móvil, monitorización de comportamiento anómalo, alertas de banca electrónica y políticas corporativas de seguridad para móviles.  |

## **Caso Real**

| Parámetro | Contenido |
| ----- | ----- |
| **URL** | [https://securelist.com/it-threat-evolution-q1-2024-mobile-statistics/112750/ ](https://securelist.com/it-threat-evolution-q1-2024-mobile-statistics/112750/)   |
| **Breve Descripción** | El informe de Kaspersky describe un troyano bancario para Android detectado en Corea que se hacía pasar por una aplicación legítima, ocultaba su icono tras la instalación y seguía ejecutándose para robar SMS, contactos, fotos y certificados digitales usados en banca online, comprometiendo gravemente las cuentas bancarias de los usuarios afectados.    |
| **Agrupación/Tipo** | Contenido malicioso \> Sistema infectado con malware |
| **Origen** | Externo |
| **Perfiles Afectados** | Usuarios de banca online móvil, empleados y clientes que utilizan certificados digitales y SMS de verificación para operaciones financieras.    |
| **Nº y Tipología Sistemas** | Dispositivos Android de usuarios en Corea que instalaron la app trojanizada, número no público pero incluido dentro del conjunto de miles de dispositivos afectados por troyanos bancarios en el periodo estudiado.    |
| **Categoría Sistemas** | Crítica (afecta a sistemas que gestionan credenciales bancarias y operaciones financieras).    |
| **Peligrosidad** | 5 |
| **Impacto** | L5 |
| **Prioridad Asignada** | Emergencia |

## **Tipo 3: Servidor C\&C**

## **Características**

| Campo | Contenido |
| ----- | ----- |
| **Descripción** | Incidente donde se detectan servidores que actúan como centros de mando y control (Command & Control o C\&C). Estos dirigen redes de bots o malware, gestionan víctimas y reciben datos robados. |
| **Funcionamiento** | Los sistemas infectados se conectan periódicamente a uno o varios servidores C\&C para recibir órdenes, descargar módulos adicionales y exfiltrar información robada. El atacante puede cambiar la configuración y rotar servidores para evadir las defensas. |
| **Identificación** | Se detecta tráfico TLS o HTTPS hacia IPs/dominios en listas IOC de campañas, uso de puertos inusuales, patrones de beaconing periódico, alertas de equipos de threat intel y correlaciones en logs de firewall o proxy. |
| **Protección** | Bloqueo de indicadores de compromiso, segmentación de red, inspección profunda de tráfico, listas de denegación actualizadas, sistemas EDR, colaboración con CERT/LEA para desmantelar la infraestructura y actualizaciones de firmas. |

## **Caso Real**

| Parámetro | Contenido |
| ----- | ----- |
| **URL** | [https://www.europol.europa.eu/media-press/newsroom/news/end-of-game-for-cybercrime-infrastructure-1025-servers-taken-down europol.europa](https://www.europol.europa.eu/media-press/newsroom/news/end-of-game-for-cybercrime-infrastructure-1025-servers-taken-down)​ |
| **Breve Descripción** | En noviembre de 2025, Europol coordinó la operación 'Endgame', desmantelando 1.025 servidores de C\&C para redes de malware como Rhadamanthys, VenomRAT y Elysium. Esto afectó a cientos de miles de equipos infectados y millones de credenciales robadas gestionadas por esa infraestructura criminal. |
| **Agrupación/Tipo** | Contenido malicioso \> Servidor C\&C |
| **Origen** | Externo |
| **Perfiles Afectados** | Usuarios finales, empresas y organismos cuyos sistemas formaban parte de las botnets controladas por esos servidores, incluidos perfiles administrativos y directivos en diversas organizaciones. |
| **Nº y Tipología Sistemas** | 1.025 servidores de C\&C desmantelados y cientos de miles de equipos de usuario y servidores comprometidos que se comunicaban con ellos.  |
| **Categoría Sistemas** | Crítica (infraestructura central para el control de botnets y campañas de malware). |
| **Peligrosidad** | 5 |
| **Impacto** | L5 |
| **Prioridad Asignada** | Emergencia |

## **Tipo 4: Distribución de malware**

## **Características**

| Campo | Contenido |
| ----- | ----- |
| **Descripción** | Incidente en el que recursos legítimos (web corporativa, cuentas en plataformas de vídeo, servicios de almacenamiento, etc.) se usan para distribuir malware, ya sea comprometiendo dichos recursos o abusando de ellos para alojar o enlazar contenido malicioso. |
| **Funcionamiento** | El atacante compromete cuentas o sitios legítimos y publica contenido atractivo (por ejemplo, cracks, herramientas, mods) que enlaza a archivos ejecutables o instaladores trojanizados que descargan y ejecutan malware en los equipos de las víctimas. |
| **Identificación** | Aparición de contenido no autorizado en canales oficiales, quejas de usuarios, detecciones de antivirus al descargar archivos desde dominios legítimos, análisis de enlaces en descripciones de vídeos o posts y correlación con campañas conocidas. |
| **Protección** | Doble factor en cuentas, revisiones de contenido, monitorización de cambios, listas de bloqueo de URLs maliciosas, formación de usuarios para desconfiar de cracks/hacks y análisis automático de archivos compartidos en plataformas corporativas. |

## **Caso Real**

| Parámetro | Contenido |
| ----- | ----- |
| **URL** | [https://research.checkpoint.com/2025/youtube-ghost-network/ research.checkpoint](https://research.checkpoint.com/2025/youtube-ghost-network/)​ |
| **Breve Descripción** | Check Point descubrió la campaña “YouTube Ghost Network”, en la que los atacantes comprometían cuentas legítimas de YouTube para subir vídeos que promocionan supuestos hacks para juegos como Roblox o cracks de Photoshop 2025 y enlazaban a instaladores trojanizados que distribuían HijackLoader y el infostealer Rhadamanthys, convirtiendo la propia plataforma de YouTube en canal de distribución masiva de malware. |
| **Agrupación/Tipo** | Contenido malicioso \> Distribución de malware |
| **Origen** | Externo |
| **Perfiles Afectados** | Usuarios generales de internet, jugadores y personas que buscan software pirata, incluyendo potencialmente empleados que descargan esos recursos desde equipos corporativos. |
| **Nº y Tipología Sistemas** | Más de 3.000 vídeos maliciosos y un número elevado de equipos de usuario que descargaron y ejecutaron los instaladores infectados, principalmente PCs con sistemas de escritorio. |
| **Categoría Sistemas** | Alta (afecta a un gran número de equipos de usuario, tanto personales como corporativos). |
| **Peligrosidad** | 4 |
| **Impacto** | L4 |
| **Prioridad Asignada** | Alta |


## **DOCUMENTACIÓN COMPLETA \- AGRUPACIÓN 2 (Intento de intrusión)**

## **Tipo 1: Explotación de vulnerabilidades conocidas (CVE)**

## **Características**

| Campo | Contenido |
| ----- | ----- |
| **Descripción** | Intento de compromiso de sistemas mediante explotación de vulnerabilidades conocidas y documentadas (con identificador CVE y puntuación CVSS) en software de servidores, dispositivos de red o aplicaciones. |
| **Funcionamiento** | El atacante escanea sistemas en busca de versiones vulnerables, aplica exploits públicos o privados para ejecutar código remoto (RCE), escalar privilegios o causar denegaciones de servicio (DoS), y despliega backdoors o herramientas de post-explotación. |
| **Identificación** | Patrones de explotación en logs (payloads específicos, errores de deserialización o RCE), alertas de IDS/IPS/EDR y comparación de versiones expuestas con listas de CVE activas. |
| **Protección** | Gestión prioritaria de parches, inventario de activos actualizado, reducción de superficie de ataque, WAF/IPS, hardening de sistemas y monitorización continua de escaneos/exploits. |

## **Caso Real**

| Parámetro | Contenido |
| ----- | ----- |
| **URL** | [https://www. .com/top-20-most-exploited-vulnerabilities-of-2025-a-comprehensive-analysis/ ](https://www.cryptika.com/top-20-most-exploited-vulnerabilities-of-2025-a-comprehensive-analysis/) ​ |
| **Breve Descripción** | En 2025, la vulnerabilidad crítica CVE-2025-5086 en DELMIA Apriso (Dassault Systèmes) permitió la deserialización de datos no confiables (CVSS 9.0). Explotada activamente vía requests SOAP antes del parche de junio, puso en riesgo sistemas OT de fabricación con ejecución remota de código. |
| **Agrupación/Tipo** | Intento de intrusión \> Exploitación de vulnerabilidades conocidas |
| **Origen** | Externo |
| **Perfiles Afectados** | Personal de operaciones de planta, administradores de sistemas industriales y dirección de fábricas que dependen de DELMIA Apriso para la gestión de procesos. |
| **Nº y Tipología Sistemas** | Múltiples instalaciones de DELMIA Apriso Release 2020 a Release 2025 desplegadas en entornos de fabricación, con servidores de aplicaciones y bases de datos afectados. |
| **Categoría Sistemas** | Crítica (sistemas OT/industriales que soportan procesos de fabricación). |
| **Peligrosidad** | 5 |
| **Impacto** | L5 |
| **Prioridad Asignada** | Emergencia |

## **Tipo 2: Explotación de vulnerabilidades conocidas (zero‑day posteriormente documentado)**

## **Características**

| Campo | Contenido |
| ----- | ----- |
| **Descripción** | Ataque informático que aprovecha fallos de seguridad en software específico. Estos fallos se explotan inicialmente cuando aún son desconocidos (vulnerabilidades de día cero), pero más adelante se registran oficialmente, se les asigna un código de identificación y pasan a formar parte del catálogo de vulnerabilidades reconocidas públicamente. |
| **Funcionamiento** | Actores avanzados descubren fallos en dispositivos de acceso remoto o seguridad perimetral, desarrollan exploits privados y los usan para obtener acceso inicial a redes corporativas, desplegando webshells y herramientas de persistencia antes de que el fabricante publique parches.​ |
| **Identificación** | Actividad sospechosa en dispositivos perimetrales, creación de archivos webshell, conexiones inusuales a paneles de administración y correlación posterior con avisos de fabricantes y análisis de incidentes de empresas de seguridad. |
| **Protección** | Segmentación, monitorización de dispositivos de borde, aplicación rápida de parches una vez publicados, reglas de detección de webshells y revisiones periódicas de integridad de sistemas.​ |

## **Caso Real**

| Parámetro | Contenido |
| ----- | ----- |
| **URL** | [https://deepstrike.io/blog/zero-day-exploit-statistics-2025 deepstrike](https://deepstrike.io/blog/zero-day-exploit-statistics-2025)​ |
| **Breve Descripción** | Un análisis de zero‑days de 2025 describe una campaña en la que actores Estado‑nación explotaron vulnerabilidades desconocidas en productos de Ivanti, obteniendo acceso a gateways perimetrales desde al menos diciembre de 2023 y desplegando webshells como LIGHTWIRE, WIREFIRE y BUSHWALK para mantener persistencia y robar configuraciones de dispositivos y credenciales. |
| **Agrupación/Tipo** | Intento de intrusión \> Exploitación de vulnerabilidades conocidas (zero‑day que después se documenta) |
| **Origen** | Externo |
| **Perfiles Afectados** | Administradores de red y seguridad, usuarios corporativos que se conectan a través de gateways Ivanti y personal de TI responsable de la infraestructura perimetral. |
| **Nº y Tipología Sistemas** | Múltiples dispositivos de acceso remoto Ivanti desplegados en entornos empresariales y gubernamentales, utilizados como punto de entrada a redes internas. |
| **Categoría Sistemas** | Crítica (infraestructura de acceso remoto y seguridad perimetral). |
| **Peligrosidad** | 5 |
| **Impacto** | L5 |
| **Prioridad Asignada** | Emergencia |

## **Tipo 3: Intento de acceso con vulneración de credenciales (fuerza bruta y credential stuffing)**

## **Características**

| Campo | Contenido |
| ----- | ----- |
| **Descripción** | Intentos masivos de acceso no autorizado mediante fuerza bruta, password spraying o credential stuffing con credenciales filtradas y débiles. |
| **Funcionamiento** | El atacante automatiza miles de intentos de login contra VPN, RDP o apps web usando listas de contraseñas populares o pares usuario/contraseña robados, buscando cuentas con credenciales reutilizadas o débiles. |
| **Identificación** | Picos de autenticaciones fallidas, patrones desde IPs inusuales/geolocalizaciones raras, detección de bots automatizados, cuentas temporalmente bloqueadas y coincidencias con brechas de credenciales en dark web. |
| **Protección** | MFA obligatoria, límites de intentos de login, detección de anomalías en accesos, contraseñas únicas y fuertes por cuenta, gestores de passwords y monitorización proactiva de comportamiento sospechoso.  |

## **Caso Real**

| Parámetro | Contenido |
| ----- | ----- |
| **URL** | [https://www.blackfog.com/brute-force-attacks-in-2025-how-they-work-whats-changed-and-how-to-stop-them/ blackfog](https://www.blackfog.com/brute-force-attacks-in-2025-how-they-work-whats-changed-and-how-to-stop-them/)​ |
| **Breve Descripción** | Informe de BlackFog (2025) sobre cómo brute force, credential stuffing y password spraying han evolucionado con IA y credenciales filtradas, atacando masivamente VPN, RDP y cloud con \>2.8M IPs en campañas globales contra edge devices. |
| **Agrupación/Tipo** | Intento de intrusión \> Intento de acceso con vulneración de credenciales |
| **Origen** | Externo |
| **Perfiles Afectados** | Empleados corporativos de todos los niveles (usuarios generales, personal administrativo y dirección) cuyas cuentas se exponen a intentos de acceso no autorizado. |
| **Nº y Tipología Sistemas** | Gran número de cuentas en servicios VPN, RDP y aplicaciones SaaS corporativas atacadas de forma continua a nivel global, sin cifra exacta pero con una tendencia creciente según el informe. |
| **Categoría Sistemas** | Alta (servicios de autenticación corporativa y acceso remoto). |
| **Peligrosidad** | 4 |
| **Impacto** | L4 |
| **Prioridad Asignada** | Alta |

## **Tipo 4: Intento de acceso con vulneración de credenciales (password spraying / reverse brute force)**

## **Características**

| Campo | Contenido |
| ----- | ----- |
| **Descripción** | Ataques que prueban pocas contraseñas comunes contra muchas cuentas (password spraying) o buscan usuarios que compartan una contraseña conocida (reverse brute force), evitando bloqueos por intentos excesivos en una sola cuenta. |
| **Funcionamiento** | Los atacantes utilizan diccionarios de contraseñas populares y listas de usuarios corporativos, distribuyendo los intentos a lo largo del tiempo y las cuentas para mantenerse por debajo de umbrales de bloqueo y detección, hasta encontrar combinaciones válidas. |
| **Identificación** | Intentos fallidos distribuidos entre múltiples cuentas, picos horarios inusuales y contraseñas comunes detectadas en logs de autenticación. |
| **Protección** | Contraseñas únicas y robustas por cuenta, MFA obligatoria, detección de patrones de spraying, bloqueo adaptativo por IP/reputación y revisión diaria de logs críticos.  |

## **Caso Real**

| Parámetro | Contenido |
| ----- | ----- |
| **URL** | [https://www.blackfog.com/brute-force-attacks-in-2025-how-they-work-whats-changed-and-how-to-stop-them/ blackfog](https://www.blackfog.com/brute-force-attacks-in-2025-how-they-work-whats-changed-and-how-to-stop-them/)​ |
| **Breve Descripción** | El mismo informe de BlackFog señala el uso intensivo de password spraying y reverse brute force a escala global contra portales VPN, RDP y aplicaciones web empresariales, distribuyendo los intentos de login entre muchas cuentas y pocas contraseñas para evitar mecanismos de bloqueo, lo que genera un elevado volumen de eventos de autenticación sospechosos en organizaciones de todo tipo. |
| **Agrupación/Tipo** | Intento de intrusión \> Intento de acceso con vulneración de credenciales |
| **Origen** | Externo |
| **Perfiles Afectados** | Usuarios generales, personal técnico y directivos cuyas cuentas se encuentran expuestas en directorios corporativos o son fácilmente identificables por su correo electrónico. |
| **Nº y Tipología Sistemas** | Múltiples servicios de autenticación corporativa, portales VPN y sistemas de acceso remoto expuestos en internet, pertenecientes a numerosas organizaciones. |
| **Categoría Sistemas** | Alta |
| **Peligrosidad** | 4 |
| **Impacto** | L3–L4 (dependiendo de si se produce una intrusión efectiva o solo intentos detectados). |
| **Prioridad Asignada** | Alta |

##  **Registro de Commits por Usuario**

Dado que se trata de un documento de texto, el equipo ha trabajado de manera colaborativa mediante Google Docs, herramienta que facilita la edición simultánea en tiempo real.

 Una vez completado, se ha subido la versión definitiva al repositorio de GitHub.

##  **Checklist de Completitud**

* 2 agrupaciones seleccionadas  
* 4 tipos por agrupación \= 8 tipos totales  
* Cada tipo tiene tabla de características (4 campos)  
* Cada tipo tiene caso real documentado (10 parámetros)  
* URLs verificables en casos reales  
* Datos del grupo completados  
* Commits de cada miembro registrados  
* Repositorio público en GitHub  
* Push completado


