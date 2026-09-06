# Security Policy

## Reporting a Vulnerability

Do not report security vulnerabilities through public GitHub Issues.

Report suspected vulnerabilities privately to the project maintainers.

Please include, when possible:

- A description of the vulnerability.
- Steps to reproduce the issue.
- The potential impact.
- Any suggested mitigation.

Do not publicly disclose a vulnerability until the project maintainers have had an opportunity to investigate it.

## Sensitive Information

Never commit sensitive information to the repository, including:

- Passwords or authentication credentials.
- API keys or access tokens.
- OAuth client secrets.
- Database credentials.
- Private keys.
- Production environment variables.
- Private student, alumni, or user data.

Use environment variables or an approved secret-management mechanism for sensitive configuration.

Example environment files may document required variables but must not contain real credentials.

## Exposed Credentials

If a credential is accidentally committed or exposed, treat it as compromised.

Revoke or rotate the credential immediately and notify the project maintainers. Removing the credential in a later commit is not sufficient because it may remain in Git history.

## Security Practices

Contributors should:

- Keep dependencies reasonably current.
- Address security alerts and dependency vulnerabilities promptly.
- Avoid disabling repository security protections without team approval.
- Follow least-privilege principles when working with accounts, APIs, and application permissions.
- Avoid using real user data for development or testing.