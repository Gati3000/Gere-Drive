# Clients
One folder per client, named with a 6-digit ID (000001, 000002, ...). Real client data is never committed, only this README and `_Template`.

| File | Content |
|---|---|
| Client.yml | name, surname, company, tax_id, whatsapp, phones, email, language, holded_contact_id, status, notes |
| Addresses.yml | list of addresses, one marked default, used for shipping labels |
| Purchases.jsonl | one purchase per line (date, document, items), append only |
| Shipments.jsonl | one shipping label per line (carrier, tracking, weight, packages, status), append only |

Postal codes and phone numbers are always quoted strings, so YAML does not cut leading zeros.
