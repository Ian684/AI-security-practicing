# Methodology and responsible use

These notes study how language models respond to instruction conflicts,
prompt injection, information-extraction requests, and unsafe tool-oriented
instructions.

For each experiment, record:

1. The challenge URL and version, when available.
2. The intended system behavior and the threat being tested.
3. The exact input and the observed output.
4. Why the input was effective or ineffective.
5. The security impact and a possible defensive control.
6. Whether the result depends on a specific model or challenge version.

Useful defensive controls to consider include instruction isolation, explicit
trust boundaries, least-privilege tool access, confirmation before external
side effects, output validation, and not exposing secrets in model context.

Only run these experiments against systems where you have permission. Do not
reuse prompts to extract secrets, send messages, alter records, bypass access
controls, or deliver phishing content on real services. Redact credentials,
private data, and non-public URLs before publishing notes.
