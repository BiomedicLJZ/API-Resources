# Security Policy

## Supported Versions

This is an educational project (API Archetypes Field Guide). There are no versioned releases with security maintenance windows — the `main` branch is always the current supported version.

| Version | Supported |
| ------- | --------- |
| main    | ✅ Yes    |

## Reporting a Vulnerability

If you discover a security vulnerability in this project, please follow responsible disclosure:

1. **Do not open a public GitHub issue** for the vulnerability.
2. Email the maintainer at **leonardo.juarez.zucco@gmail.com** with the subject line `[SECURITY] <brief description>`.
3. Include in your report:
   - A description of the vulnerability
   - Steps to reproduce it
   - Potential impact
   - Any suggested fix (optional but appreciated)

You can expect an acknowledgement within **72 hours** and a resolution or status update within **14 days**.

## Scope

Since this is a front-end only educational application with no backend, database, or user authentication, the attack surface is limited. Relevant areas include:

- **Dependency vulnerabilities** — run `npm audit` to check
- **Supply chain attacks** — malicious packages in `node_modules`
- **XSS** — no `dangerouslySetInnerHTML` is used in this project

## Security Notes for the Code Examples

The code samples in this guide are **for educational purposes**. When adapting them for production, always:

- Validate and sanitize all user inputs at system boundaries
- Use HTTPS in production (never `grpc.insecure_channel()` or `http://` in gRPC)
- Store secrets in environment variables, never in source code
- Verify HMAC signatures on all incoming webhooks before processing
- Use `hmac.compare_digest()` (Python) or `crypto.timingSafeEqual()` (Node.js) to prevent timing attacks on signature comparisons
- For SOAP: always use WS-Security with transport-level TLS and validate the WSDL source
