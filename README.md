# Ledgebrook

Ledgebrook is a technology-enabled excess and surplus (E&S) lines managing general agent (MGA) and
reinsurance platform founded by Gage Caligaris and headquartered in Massachusetts. It underwrites
specialty commercial casualty risk — general liability, professional liability, and cyber —
exclusively through wholesale brokers, competing on quoting speed rather than direct-to-consumer
distribution. Ledgebrook Re extends the business into delegated-authority reinsurance from London
and Dubai.

- https://www.ledgebrook.com/
- https://forgeglobal.com/ledgebrook_stock/ (secondary market listing)

## API surface

Ledgebrook publishes **no public API, developer portal, or machine-readable API contract**. Contract
discovery (OpenAPI, GraphQL, MCP, A2A agent card, `/.well-known/*`, package registries, GitHub) was
run against every resolvable host and returned no hits — see
[`well-known/ledgebrook-well-known.yml`](well-known/ledgebrook-well-known.yml) for the full probe
record. Its broker quoting platform and underwriting workbench are private, credentialed surfaces,
and policy administration runs on Socotra Connected Core; the "open APIs" cited in that partnership
are Socotra's, catalogued under the Socotra provider.

## Artifacts

| Artifact | File | Method |
|---|---|---|
| Well-Known / contract discovery | `well-known/ledgebrook-well-known.yml` | probed |
| Domain security | `security/ledgebrook-domain-security.yml` | probed |
| llms.txt | `llms/ledgebrook-llms.txt` | generated |
