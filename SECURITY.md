# Security Policy

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| 1.x.x   | :white_check_mark: |
| < 1.0   | :x:                |

## Reporting a Vulnerability

We take security seriously. If you discover a security vulnerability, please follow these steps:

1. **Do NOT open a public issue** - This could expose the vulnerability to malicious actors
2. **Email us directly** at security@your-domain.com with:
   - Description of the vulnerability
   - Steps to reproduce
   - Potential impact
   - Suggested fix (if any)

3. **Allow us time to respond**:
   - Initial response within 48 hours
   - Regular updates on progress
   - Credit you in the advisory (unless you prefer anonymity)

## Security Measures

This project implements the following security practices:

- **Dependency scanning**: Automated via GitHub Dependabot
- **Code scanning**: GitHub CodeQL analysis on every PR
- **Secret detection**: GitHub secret scanning enabled
- **Input validation**: All user inputs validated via Zod schemas
- **SQL injection prevention**: Prisma ORM with parameterized queries
- **XSS protection**: React's built-in escaping + CSP headers
- **CSRF protection**: NextAuth.js built-in CSRF tokens
- **Rate limiting**: Implemented on API routes
- **HTTPS enforcement**: HSTS headers in production

## Best Practices for Users

1. Keep dependencies updated (`npm audit fix`)
2. Use strong, unique passwords
3. Enable 2FA on your accounts
4. Regularly review access permissions
5. Report suspicious activity immediately

## Security Updates

Security patches are released as soon as possible after vulnerability confirmation. Users are notified via:
- GitHub Security Advisories
- Release notes
- Email notifications (if subscribed)

## Acknowledgments

We thank the following security researchers who have responsibly disclosed vulnerabilities:

- [Your Name] - [Vulnerability Description] - [Date]

## Contact

- Security Team: security@your-domain.com
- PGP Key: [Link to PGP key]
- Response Time: < 48 hours
