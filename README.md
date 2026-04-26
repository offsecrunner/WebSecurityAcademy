# WebSecurityAcademy

# PortSwigger Web Security Academy – Complete Labs Checklist (2026)
- [Mystery Lab Challenge](#mystery-lab-challenge)
- [SQL Injection](#sql-injection)
- [Cross-site Scripting (XSS)](#cross-site-scripting-xss)
- [Cross-site Request Forgery (CSRF)](#cross-site-request-forgery-csrf)
- [Clickjacking](#clickjacking)
- [DOM-based Vulnerabilities](#dom-based-vulnerabilities)
- [Cross-origin Resource Sharing (CORS)](#cross-origin-resource-sharing-cors)
- [XML External Entity (XXE) Injection](#xml-external-entity-xxe-injection)
- [Server-side Request Forgery (SSRF)](#server-side-request-forgery-ssrf)
- [HTTP Request Smuggling](#http-request-smuggling)
- [OS Command Injection](#os-command-injection)
- [Server-side Template Injection](#server-side-template-injection)
- [Path Traversal](#path-traversal)
- [Access Control Vulnerabilities](#access-control-vulnerabilities)
- [Authentication](#authentication)
- [WebSockets](#websockets)
- [Web Cache Poisoning](#web-cache-poisoning)
- [Insecure Deserialization](#insecure-deserialization)
- [Information Disclosure](#information-disclosure)
- [Business Logic Vulnerabilities](#business-logic-vulnerabilities)
- [HTTP Host Header Attacks](#http-host-header-attacks)
- [OAuth Authentication](#oauth-authentication)
- [File Upload Vulnerabilities](#file-upload-vulnerabilities)
- [JWT Attacks](#jwt-attacks)
- [Essential Skills](#essential-skills)
- [Prototype Pollution](#prototype-pollution)
- [GraphQL API Vulnerabilities](#graphql-api-vulnerabilities)
- [Race Conditions](#race-conditions)
- [NoSQL Injection](#nosql-injection)
- [API Testing](#api-testing)
- [Web LLM Attacks](#web-llm-attacks)
- [Web Cache Deception](#web-cache-deception)

## Mystery Lab Challenge
- [ ] Mystery lab challenge

## SQL Injection
- [x] SQL injection vulnerability in WHERE clause allowing retrieval of hidden data (Apprentice)
- [x] SQL injection vulnerability allowing login bypass (Apprentice)
- [ ] SQL injection attack, querying the database type and version on Oracle (Practitioner)
- [ ] SQL injection attack, querying the database type and version on MySQL and Microsoft (Practitioner)
- [ ] SQL injection attack, listing the database contents on non-Oracle databases (Practitioner)
- [ ] SQL injection attack, listing the database contents on Oracle (Practitioner)
- [ ] SQL injection UNION attack, determining the number of columns returned by the query (Practitioner)
- [ ] SQL injection UNION attack, finding a column containing text (Practitioner)
- [ ] SQL injection UNION attack, retrieving data from other tables (Practitioner)
- [ ] SQL injection UNION attack, retrieving multiple values in a single column (Practitioner)
- [ ] Blind SQL injection with conditional responses (Practitioner)
- [ ] Blind SQL injection with conditional errors (Practitioner)
- [ ] Visible error-based SQL injection (Practitioner)
- [ ] Blind SQL injection with time delays (Practitioner)
- [ ] Blind SQL injection with time delays and information retrieval (Practitioner)
- [ ] Blind SQL injection with out-of-band interaction (Practitioner)
- [ ] Blind SQL injection with out-of-band data exfiltration (Practitioner)
- [ ] SQL injection with filter bypass via XML encoding (Practitioner)

## Cross-site Scripting (XSS)
### Apprentice
- [ ] Reflected XSS into HTML context with nothing encoded
- [ ] Stored XSS into HTML context with nothing encoded
- [ ] DOM XSS in document.write sink using source location.search
- [ ] DOM XSS in innerHTML sink using source location.search
- [ ] DOM XSS in jQuery anchor href attribute sink using location.search source
- [ ] DOM XSS in jQuery selector sink using a hashchange event
- [ ] Reflected XSS into attribute with angle brackets HTML-encoded
- [ ] Stored XSS into anchor href attribute with double quotes HTML-encoded
- [ ] Reflected XSS into a JavaScript string with angle brackets HTML encoded

### Practitioner
- [x] DOM XSS in document.write sink using source location.search inside a select element
- [ ] DOM XSS in AngularJS expression with angle brackets and double quotes HTML-encoded
- [ ] Reflected DOM XSS
- [ ] Stored DOM XSS
- [ ] Reflected XSS into HTML context with most tags and attributes blocked
- [ ] Reflected XSS into HTML context with all tags blocked except custom ones
- [ ] Reflected XSS with some SVG markup allowed
- [ ] Reflected XSS in canonical link tag
- [ ] Reflected XSS into a JavaScript string with single quote and backslash escaped
- [ ] Reflected XSS into a JavaScript string with angle brackets and double quotes HTML-encoded and single quotes escaped
- [ ] Stored XSS into onclick event with angle brackets and double quotes HTML-encoded and single quotes and backslash escaped
- [ ] Reflected XSS into a template literal with angle brackets, single, double quotes, backslash and backticks Unicode-escaped
- [ ] Exploiting cross-site scripting to steal cookies
- [ ] Exploiting cross-site scripting to capture passwords
- [ ] Exploiting XSS to bypass CSRF defenses
- [ ] Reflected XSS protected by very strict CSP, with dangling markup attack

### Expert
- [ ] Reflected XSS with AngularJS sandbox escape without strings
- [ ] Reflected XSS with AngularJS sandbox escape and CSP
- [ ] Reflected XSS with event handlers and href attributes blocked
- [ ] Reflected XSS in a JavaScript URL with some characters blocked
- [ ] Reflected XSS protected by CSP, with CSP bypass

## Cross-site Request Forgery (CSRF)
- [ ] CSRF vulnerability with no defenses (Apprentice)
- [ ] CSRF where token validation depends on request method (Practitioner)
- [ ] CSRF where token validation depends on token being present (Practitioner)
- [ ] CSRF where token is not tied to user session (Practitioner)
- [ ] CSRF where token is tied to non-session cookie (Practitioner)
- [ ] CSRF where token is duplicated in cookie (Practitioner)
- [ ] SameSite Lax bypass via method override (Practitioner)
- [ ] SameSite Strict bypass via client-side redirect (Practitioner)
- [ ] SameSite Strict bypass via sibling domain (Practitioner)
- [ ] SameSite Lax bypass via cookie refresh (Practitioner)
- [ ] CSRF where Referer validation depends on header being present (Practitioner)
- [ ] CSRF with broken Referer validation (Practitioner)

## Clickjacking
- [ ] Basic clickjacking with CSRF token protection (Apprentice)
- [ ] Clickjacking with form input data prefilled from a URL parameter (Apprentice)
- [ ] Clickjacking with a frame buster script (Apprentice)
- [ ] Exploiting clickjacking vulnerability to trigger DOM-based XSS (Practitioner)
- [ ] Multistep clickjacking (Practitioner)

## DOM-based Vulnerabilities
- [ ] DOM XSS using web messages (Practitioner)
- [ ] DOM XSS using web messages and a JavaScript URL (Practitioner)
- [ ] DOM XSS using web messages and JSON.parse (Practitioner)
- [ ] DOM-based open redirection (Practitioner)
- [ ] DOM-based cookie manipulation (Practitioner)
- [ ] Exploiting DOM clobbering to enable XSS (Expert)
- [ ] Clobbering DOM attributes to bypass HTML filters (Expert)

## Cross-origin Resource Sharing (CORS)
- [ ] CORS vulnerability with basic origin reflection (Apprentice)
- [ ] CORS vulnerability with trusted null origin (Apprentice)
- [ ] CORS vulnerability with trusted insecure protocols (Practitioner)

## XML External Entity (XXE) Injection
- [ ] Exploiting XXE using external entities to retrieve files (Apprentice)
- [ ] Exploiting XXE to perform SSRF attacks (Apprentice)
- [ ] Blind XXE with out-of-band interaction (Practitioner)
- [ ] Blind XXE with out-of-band interaction via XML parameter entities (Practitioner)
- [ ] Exploiting blind XXE to exfiltrate data using a malicious external DTD (Practitioner)
- [ ] Exploiting blind XXE to retrieve data via error messages (Practitioner)
- [ ] Exploiting XInclude to retrieve files (Practitioner)
- [ ] Exploiting XXE via image file upload (Practitioner)
- [ ] Exploiting XXE to retrieve data by repurposing a local DTD (Expert)

## Server-side Request Forgery (SSRF)
- [X] Basic SSRF against the local server (Apprentice)  | [Youtube Video](https://youtu.be/p0Z8Acazrbg)
- [X] Basic SSRF against another back-end system (Apprentice) | [Youtube Video](https://youtu.be/7yT6-DUsFGI)
- [X] Blind SSRF with out-of-band detection (Practitioner) | [Youtube Video](https://youtu.be/GPTsEDPb39g)
- [X] SSRF with blacklist-based input filter (Practitioner) | [Youtube Video](https://youtu.be/TWc1MSIzsIk)
- [X] SSRF with filter bypass via open redirection vulnerability (Practitioner) | [Youtube Video](https://youtu.be/lOks4NwXHbs)
- [X] Blind SSRF with Shellshock exploitation (Expert) | [Youtube Video](https://youtu.be/B24vApdWB4s)
- [X] SSRF with whitelist-based input filter (Expert) | [Youtube Video](https://youtu.be/QFr0kzQLSFM)

## HTTP Request Smuggling
- [ ] HTTP request smuggling, confirming a CL.TE vulnerability via differential responses (Practitioner)
- [ ] HTTP request smuggling, confirming a TE.CL vulnerability via differential responses (Practitioner)
- [ ] Exploiting HTTP request smuggling to bypass front-end security controls, CL.TE vulnerability (Practitioner)
- [ ] Exploiting HTTP request smuggling to bypass front-end security controls, TE.CL vulnerability (Practitioner)
- [ ] Exploiting HTTP request smuggling to reveal front-end request rewriting (Practitioner)
- [ ] Exploiting HTTP request smuggling to capture other users' requests (Practitioner)
- [ ] Exploiting HTTP request smuggling to deliver reflected XSS (Practitioner)
- [ ] Response queue poisoning via H2.TE request smuggling (Practitioner)
- [ ] H2.CL request smuggling (Practitioner)
- [ ] HTTP/2 request smuggling via CRLF injection (Practitioner)
- [ ] HTTP/2 request splitting via CRLF injection (Practitioner)
- [ ] 0.CL request smuggling (Expert)
- [ ] CL.0 request smuggling (Practitioner)
- [ ] HTTP request smuggling, basic CL.TE vulnerability (Practitioner)
- [ ] HTTP request smuggling, basic TE.CL vulnerability (Practitioner)
- [ ] HTTP request smuggling, obfuscating the TE header (Practitioner)
- [ ] Exploiting HTTP request smuggling to perform web cache poisoning (Expert)
- [ ] Exploiting HTTP request smuggling to perform web cache deception (Expert)
- [ ] Bypassing access controls via HTTP/2 request tunnelling (Expert)
- [ ] Web cache poisoning via HTTP/2 request tunnelling (Expert)
- [ ] Client-side desync (Expert)
- [ ] Server-side pause-based request smuggling (Expert)

## OS Command Injection
- [ ] OS command injection, simple case (Apprentice)
- [ ] Blind OS command injection with time delays (Practitioner)
- [ ] Blind OS command injection with output redirection (Practitioner)
- [ ] Blind OS command injection with out-of-band interaction (Practitioner)
- [ ] Blind OS command injection with out-of-band data exfiltration (Practitioner)

## Server-side Template Injection
- [ ] Basic server-side template injection (Practitioner)
- [ ] Basic server-side template injection (code context) (Practitioner)
- [ ] Server-side template injection using documentation (Practitioner)
- [ ] Server-side template injection in an unknown language with a documented exploit (Practitioner)
- [ ] Server-side template injection with information disclosure via user-supplied objects (Practitioner)
- [ ] Server-side template injection in a sandboxed environment (Expert)
- [ ] Server-side template injection with a custom exploit (Expert)

## Path Traversal
- [ ] File path traversal, simple case (Apprentice)
- [ ] File path traversal, traversal sequences blocked with absolute path bypass (Practitioner)
- [ ] File path traversal, traversal sequences stripped non-recursively (Practitioner)
- [ ] File path traversal, traversal sequences stripped with superfluous URL-decode (Practitioner)
- [ ] File path traversal, validation of start of path (Practitioner)
- [ ] File path traversal, validation of file extension with null byte bypass (Practitioner)

## Access Control Vulnerabilities
- [ ] Unprotected admin functionality (Apprentice)
- [ ] Unprotected admin functionality with unpredictable URL (Apprentice)
- [ ] User role controlled by request parameter (Apprentice)
- [ ] User role can be modified in user profile (Apprentice)
- [ ] User ID controlled by request parameter (Apprentice)
- [ ] User ID controlled by request parameter, with unpredictable user IDs (Apprentice)
- [ ] User ID controlled by request parameter with data leakage in redirect (Apprentice)
- [ ] User ID controlled by request parameter with password disclosure (Apprentice)
- [ ] Insecure direct object references (Apprentice)
- [ ] URL-based access control can be circumvented (Practitioner)
- [ ] Method-based access control can be circumvented (Practitioner)
- [ ] Multi-step process with no access control on one step (Practitioner)
- [ ] Referer-based access control (Practitioner)

## Authentication
- [ ] Username enumeration via different responses (Apprentice)
- [ ] 2FA simple bypass (Apprentice)
- [ ] Password reset broken logic (Apprentice)
- [ ] Username enumeration via subtly different responses (Practitioner)
- [ ] Username enumeration via response timing (Practitioner)
- [ ] Broken brute-force protection, IP block (Practitioner)
- [ ] Username enumeration via account lock (Practitioner)
- [ ] 2FA broken logic (Practitioner)
- [ ] Brute-forcing a stay-logged-in cookie (Practitioner)
- [ ] Offline password cracking (Practitioner)
- [ ] Password reset poisoning via middleware (Practitioner)
- [ ] Password brute-force via password change (Practitioner)
- [ ] Broken brute-force protection, multiple credentials per request (Expert)
- [ ] 2FA bypass using a brute-force attack (Expert)

## WebSockets
- [ ] Manipulating WebSocket messages to exploit vulnerabilities (Apprentice)
- [ ] Cross-site WebSocket hijacking (Practitioner)
- [ ] Manipulating the WebSocket handshake to exploit vulnerabilities (Practitioner)

## Web Cache Poisoning
- [x] Web cache poisoning with an unkeyed header (Practitioner) | [Youtube Video](https://youtu.be/24bifds_aaU?si=hbaiAwaGIguwYySu)
- [x] Web cache poisoning with an unkeyed cookie (Practitioner) | [YouTube Video](https://youtu.be/FHWvI-If3Kg?si=HWTs6PIJuFW8m4Ly)
- [x] Web cache poisoning with multiple headers (Practitioner) | [YouTube Video](https://youtu.be/sTzNB_NzYdQ)
- [x] Targeted web cache poisoning using an unknown header (Practitioner) | [YouTube Video](https://youtu.be/fBMGCEGqAbA?si=7Awe1ERBYZ03ui9v)
- [x] Web cache poisoning via an unkeyed query string (Practitioner) | [YouTube Video](https://youtu.be/8xViXA9GPA8?si=neA0GDvOhxpg4zcp)
- [x] Web cache poisoning via an unkeyed query parameter (Practitioner) | [YouTube Video](https://youtu.be/L-SMOpuTsJM)
- [x] Parameter cloaking (Practitioner) | [YouTube Video](https://youtu.be/IPUsy_0kZxg)
- [x] Web cache poisoning via a fat GET request (Practitioner) | [YouTube Video](https://youtu.be/pLH3WUflSoY)
- [x] URL normalization (Practitioner) | [YouTube Video](https://youtu.be/wY3akcbwM-M)
- [x] Web cache poisoning to exploit a DOM vulnerability via a cache with strict cacheability criteria (Expert) | [YouTube Video](https://youtu.be/3oLrCFkREmc)
- [x] Combining web cache poisoning vulnerabilities (Expert) | [YouTube Video](https://youtu.be/W_vGb4Ts-EA)
- [x] Cache key injection (Expert) | [YouTube Video](https://youtu.be/BdEcFAH37v8)
- [x] Internal cache poisoning (Expert) | [YouTube Video](https://youtu.be/1_-R2ZOdDKE)

## Insecure Deserialization
- [x] Modifying serialized objects (Apprentice)
- [x] Modifying serialized data types (Practitioner)
- [ ] Using application functionality to exploit insecure deserialization (Practitioner)
- [ ] Arbitrary object injection in PHP (Practitioner)
- [ ] Exploiting Java deserialization with Apache Commons (Practitioner)
- [ ] Exploiting PHP deserialization with a pre-built gadget chain (Practitioner)
- [ ] Exploiting Ruby deserialization using a documented gadget chain (Practitioner)
- [ ] Developing a custom gadget chain for Java deserialization (Expert)
- [ ] Developing a custom gadget chain for PHP deserialization (Expert)
- [ ] Using PHAR deserialization to deploy a custom gadget chain (Expert)

## Information Disclosure
- [ ] Information disclosure in error messages (Apprentice)
- [ ] Information disclosure on debug page (Apprentice)
- [ ] Source code disclosure via backup files (Apprentice)
- [ ] Authentication bypass via information disclosure (Apprentice)
- [ ] Information disclosure in version control history (Practitioner)

## Business Logic Vulnerabilities
- [ ] Excessive trust in client-side controls (Apprentice)
- [ ] High-level logic vulnerability (Apprentice)
- [ ] Inconsistent security controls (Apprentice)
- [ ] Flawed enforcement of business rules (Apprentice)
- [ ] Low-level logic flaw (Practitioner)
- [ ] Inconsistent handling of exceptional input (Practitioner)
- [ ] Weak isolation on dual-use endpoint (Practitioner)
- [ ] Insufficient workflow validation (Practitioner)
- [ ] Authentication bypass via flawed state machine (Practitioner)
- [ ] Infinite money logic flaw (Practitioner)
- [ ] Authentication bypass via encryption oracle (Practitioner)
- [ ] Bypassing access controls using email address parsing discrepancies (Expert)

## HTTP Host Header Attacks
- [ ] Basic password reset poisoning (Apprentice)
- [ ] Host header authentication bypass (Apprentice)
- [ ] Web cache poisoning via ambiguous requests (Practitioner)
- [ ] Routing-based SSRF (Practitioner)
- [ ] SSRF via flawed request parsing (Practitioner)
- [ ] Host validation bypass via connection state attack (Practitioner)
- [ ] Password reset poisoning via dangling markup (Expert)

## OAuth Authentication
- [ ] Authentication bypass via OAuth implicit flow (Apprentice)
- [ ] SSRF via OpenID dynamic client registration (Practitioner)
- [ ] Forced OAuth profile linking (Practitioner)
- [ ] OAuth account hijacking via redirect_uri (Practitioner)
- [ ] Stealing OAuth access tokens via an open redirect (Practitioner)
- [ ] Stealing OAuth access tokens via a proxy page (Expert)

## File Upload Vulnerabilities
- [ ] Remote code execution via web shell upload (Apprentice)
- [ ] Web shell upload via Content-Type restriction bypass (Apprentice)
- [ ] Web shell upload via path traversal (Practitioner)
- [ ] Web shell upload via extension blacklist bypass (Practitioner)
- [ ] Web shell upload via obfuscated file extension (Practitioner)
- [ ] Remote code execution via polyglot web shell upload (Practitioner)
- [ ] Web shell upload via race condition (Expert)

## JWT Attacks
- [x] JWT authentication bypass via unverified signature (Apprentice) | [Youtube Video](https://youtu.be/PsqNWSXUSgs)
- [x] JWT authentication bypass via flawed signature verification (Apprentice) | [Youtube Video](https://youtu.be/wQeDag74fao)
- [x] JWT authentication bypass via weak signing key (Practitioner) | [Youtube Video](https://youtu.be/7W2Br3_w-5o)
- [x] JWT authentication bypass via jwk header injection (Practitioner) | [Youtube Video](https://youtu.be/Lx732We3VsA)
- [x] JWT authentication bypass via jku header injection (Practitioner) | [Youtube Video](https://youtu.be/dxi71gcwuwI)
- [x] JWT authentication bypass via kid header path traversal (Practitioner) | [Youtube Video](https://youtu.be/d7vqBAjCr_w)
- [x] JWT authentication bypass via algorithm confusion (Expert) | [Youtube Video](https://youtu.be/TKoBEFfsw9E)
- [x] JWT authentication bypass via algorithm confusion with no exposed key (Expert) | [Youtube Video](https://youtu.be/4J9EL7Bhdp4)

## Essential Skills
- [ ] Discovering vulnerabilities quickly with targeted scanning (Practitioner) | [Youtube Video]()
- [ ] Scanning non-standard data structures (Practitioner) | [Youtube Video]()

## Prototype Pollution
- [ ] Client-side prototype pollution via browser APIs (Practitioner) | [Youtube Video]()
- [ ] DOM XSS via client-side prototype pollution (Practitioner) | [Youtube Video]()
- [ ] DOM XSS via an alternative prototype pollution vector (Practitioner) | [Youtube Video]()
- [ ] Client-side prototype pollution via flawed sanitization (Practitioner) | [Youtube Video]()
- [ ] Client-side prototype pollution in third-party libraries (Practitioner) | [Youtube Video]()
- [ ] Privilege escalation via server-side prototype pollution (Practitioner) | [Youtube Video]()
- [ ] Detecting server-side prototype pollution without polluted property reflection (Practitioner) | [Youtube Video]()
- [ ] Bypassing flawed input filters for server-side prototype pollution (Practitioner) | [Youtube Video]()
- [ ] Remote code execution via server-side prototype pollution (Practitioner) | [Youtube Video]()
- [ ] Exfiltrating sensitive data via server-side prototype pollution (Expert) | [Youtube Video]()

## GraphQL API Vulnerabilities
- [ ] Accessing private GraphQL posts (Apprentice) | [Youtube Video]()
- [ ] Accidental exposure of private GraphQL fields (Practitioner) | [Youtube Video]()
- [ ] Finding a hidden GraphQL endpoint (Practitioner) | [Youtube Video]()
- [ ] Bypassing GraphQL brute force protections (Practitioner) | [Youtube Video]()
- [ ] Performing CSRF exploits over GraphQL (Practitioner) | [Youtube Video]()

## Race Conditions
- [ ] Limit overrun race conditions (Apprentice) | [Youtube Video]()
- [ ] Bypassing rate limits via race conditions (Practitioner) | [Youtube Video]()
- [ ] Multi-endpoint race conditions (Practitioner) | [Youtube Video]()
- [ ] Single-endpoint race conditions (Practitioner) | [Youtube Video]()
- [ ] Exploiting time-sensitive vulnerabilities (Practitioner) | [Youtube Video]()
- [ ] Partial construction race conditions (Expert) | [Youtube Video]()

## NoSQL Injection
- [ ] Detecting NoSQL injection (Apprentice) | [Youtube Video]()
- [ ] Exploiting NoSQL operator injection to bypass authentication (Apprentice) | [Youtube Video]()
- [ ] Exploiting NoSQL injection to extract data (Practitioner) | [Youtube Video]()
- [ ] Exploiting NoSQL operator injection to extract unknown fields (Practitioner) | [Youtube Video]()

## API Testing
- [ ] Exploiting an API endpoint using documentation (Apprentice) | [Youtube Video]()
- [ ] Exploiting server-side parameter pollution in a query string (Practitioner) | [Youtube Video]()
- [ ] Finding and exploiting an unused API endpoint (Practitioner) | [Youtube Video]()
- [ ] Exploiting a mass assignment vulnerability (Practitioner) | [Youtube Video]()
- [ ] Exploiting server-side parameter pollution in a REST URL (Expert) | [Youtube Video]()

## Web LLM Attacks
- [ ] Exploiting LLM APIs with excessive agency (Apprentice) | [Youtube Video]()
- [ ] Exploiting vulnerabilities in LLM APIs (Practitioner) | [Youtube Video]()
- [ ] Indirect prompt injection (Practitioner) | [Youtube Video]()
- [ ] Exploiting insecure output handling in LLMs (Expert) | [Youtube Video]()

## Web Cache Deception
- [ ] Exploiting path mapping for web cache deception (Apprentice) | [Youtube Video]()
- [ ] Exploiting path delimiters for web cache deception (Practitioner) | [Youtube Video]()
- [ ] Exploiting origin server normalization for web cache deception (Practitioner) | [Youtube Video]()
- [ ] Exploiting cache server normalization for web cache deception (Practitioner) | [Youtube Video]()
- [ ] Exploiting exact-match cache rules for web cache deception (Expert) | [Youtube Video]()
