# ⚠️ Disclaimer & Liability Limitation

**Use at your own risk.** The code, workflows, and scripts in this repository (`n8n-hubspot-company-legal-suffix-standardizer`) are provided for educational and architectural demonstration purposes.

## No Liability

The author and dhRobin Systems accept no responsibility or liability for any direct, indirect, incidental, or consequential damages that result from using, misusing, or deploying these scripts. This includes, without limitation, incorrectly shortened, merged or overwritten company names; loss of legal entity names needed for contracts, quotes, invoices or compliance records; broken integrations, workflows, reports or dedupe rules that depend on company names; incorrect matches with external data providers; overwritten HubSpot properties; exposure of tokens or webhook URLs; service interruptions; and API rate-limit or quota exhaustion.

## No Warranty

All software, n8n JSON blueprints, JavaScript modules and prompts are provided "AS IS", without warranty of any kind, express or implied. This includes, but is not limited to, warranties of merchantability, fitness for a particular purpose, and non-infringement.

No warranty is given that the suffix tables are complete or correct for any jurisdiction; that brand names, abbreviations or words resembling legal forms are always protected; that descriptors such as Holdings or Group are safe to remove for your records; that `match_key` values produce correct matches with any provider; that HubSpot search, pagination or batch update responses remain compatible with this workflow; or that every update succeeds.

## Production Testing Required

Always test thoroughly in an isolated staging environment, such as a HubSpot developer test account or sandbox, with `SANDBOX_MODE=true`, `DRY_RUN=true` and `WRITE_TO_HUBSPOT=false` enabled, before you connect live HubSpot credentials. Review the full list of proposed changes and refused strips in the audit, protect brand names that must not change, start with a small `BATCH_LIMIT` in preserve mode, and confirm the results on real records before running a backfill.

Treat every cleaned name as a proposed change that a person must be able to review and reverse. Do not overwrite the `name` property without a backup property and the agreement of whoever owns legal, billing and integration uses of company names.

## Third-Party APIs & Compliance

You alone are responsible for complying with the terms of service, rate limits, data privacy regulations (GDPR/CCPA and equivalents), and security policies of HubSpot, Slack, your webhook receiver, your enrichment providers and any connected services. That includes:

- granting the private app only `crm.objects.companies.read` and `crm.objects.companies.write`;
- keeping an original copy of every overwritten name and a record of every automated change;
- checking contractual, billing, tax and integration uses of company names before changing them;
- treating company names that identify individuals (for example, sole traders) as personal data;
- securing, rotating and restricting access to the HubSpot token, Slack webhook URL and alert webhook token;
- limiting access to n8n execution data and notifications, which contain company names;
- reviewing every automatically updated record.

## No Affiliation

HubSpot, Slack and n8n are trademarks of their respective owners. This project is independent and is not affiliated with, endorsed by, or sponsored by any of them. All company names and identifiers in the fixtures, sample payloads and pinned data are fictitious.

## Not Professional Advice

Nothing in this repository constitutes legal, corporate, privacy, security, or financial advice. Legal entity forms carry legal meaning; consult qualified professionals for your specific circumstances.

---

Released under the MIT License. Copyright (c) 2026 DH Robin (dhRobin Systems). See [LICENSE](LICENSE).

Full text: DISCLAIMER.md · Licensed under the MIT License. License: MIT © 2026 dhRobin Systems · Provided as-is, see the disclaimer.
