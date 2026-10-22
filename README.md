# pactlab-demo-data

This is a synthetic data set for the various pactlab pack. You can use this to test a specific pack, or download it and modify it to use real data to do deal analysis or simply point it to claude or any AI tools and learn the format and ask it to produce same format files for ur actual data to be fed into Pactlab for analysis.

> **All data here is fictional.** Every company, person, address, account number and figure is invented for demonstrations. Nothing is copied from a real business. Customers are marked “(synthetic)”; people appear only as roles, unit numbers or pseudonymous references (P07, PR-04).

## Layout

```text
<pack>/<CURRENCY>/
  README.md              the target, each file, how to load it, and the planted findings
  invoice-lines.csv      revenue lines on the Pactlab standard billing template
  <extract>.csv          pack evidence: rent rolls, T-12s, loan tapes, census, STR, …
  documents/*.pdf, *.md  agreements, reports and a paged copy of the extracts
  vdr-index.csv          the folder listed as a data room would list it
```

Each pack comes in **USD**, **EUR** and **GBP**: the same business model as a separate fictional company in the United States, the Netherlands and the United Kingdom, with its own figures. Each folder is self-consistent — the same names, dates and amounts in every file — and covers October 2024 to September 2026.

## Packs

| Pack | Fictional target | Currencies |
|---|---|---|
| [Software and SaaS](software-saas/) | Brightwave Software sells workflow software to mid-sized logistics and services firms on monthly and annual subscriptions. | [USD](software-saas/USD/) · [EUR](software-saas/EUR/) · [GBP](software-saas/GBP/) |
| [Fintech](fintech/) | Tallyport Payments runs a payments and working-capital platform for independent retailers, earning monthly platform fees and lending to merchants through a partner bank. | [USD](fintech/USD/) · [EUR](fintech/EUR/) · [GBP](fintech/GBP/) |
| [Healthcare services and healthtech](healthcare/) | Riverside Care Partners operates nine physical-therapy and primary-care practices, paid mostly by government programmes and commercial insurers. | [USD](healthcare/USD/) · [EUR](healthcare/EUR/) · [GBP](healthcare/GBP/) |
| [Telecom and media](telecom-media/) | Northlake Fibre is a regional fibre broadband and streaming-TV provider selling residential and small-business plans in four regions. | [USD](telecom-media/USD/) · [EUR](telecom-media/EUR/) · [GBP](telecom-media/GBP/) |
| [IT and professional services](professional-services/) | Sablestone Consulting is a 140-person digital and data consultancy working on monthly retainers for enterprise clients. | [USD](professional-services/USD/) · [EUR](professional-services/EUR/) · [GBP](professional-services/GBP/) |
| [Pharma and biotech](pharma-biotech/) | Calvera Pharmaceuticals is a specialty-pharma company earning royalties and supply revenue on two marketed products, with one late-stage programme. | [USD](pharma-biotech/USD/) · [EUR](pharma-biotech/EUR/) · [GBP](pharma-biotech/GBP/) |
| [E-commerce and DTC](ecommerce-dtc/) | Ridgeline Outfitters sells outdoor apparel direct to consumers through its own store, one large marketplace and a few wholesale retailers. | [USD](ecommerce-dtc/USD/) · [EUR](ecommerce-dtc/EUR/) · [GBP](ecommerce-dtc/GBP/) |
| [Hotels and hospitality](hotels/) | Harbourview Hotel Holdings owns and operates the 180-room Harbourview Hotel, a branded upscale hotel under a franchise agreement. | [USD](hotels/USD/) · [EUR](hotels/EUR/) · [GBP](hotels/GBP/) |
| [Multifamily](multifamily/) | Larkfield Residential owns Larkfield Commons, a 96-unit garden-style apartment community in three buildings (A, B, C). | [USD](multifamily/USD/) · [EUR](multifamily/EUR/) · [GBP](multifamily/GBP/) |
| [Commercial property](commercial-property/) | Quayside Estates owns Quayside Business Park, a 210,000 sq ft mixed office and light-industrial park with eleven tenants. | [USD](commercial-property/USD/) · [EUR](commercial-property/EUR/) · [GBP](commercial-property/GBP/) |
| [Hospitals](hospitals/) | St. Brennan Health operates St. Brennan Regional Medical Center, a 220-bed acute-care hospital with cardiology, orthopaedics and maternity service lines. | [USD](hospitals/USD/) · [EUR](hospitals/EUR/) · [GBP](hospitals/GBP/) |
| [Small clinics](small-clinics/) | Clearbrook Clinics runs six dental and physiotherapy clinics with 22 providers, paid by insurers and patients. | [USD](small-clinics/USD/) · [EUR](small-clinics/EUR/) · [GBP](small-clinics/GBP/) |

## Using a pack

1. Download one `<pack>/<CURRENCY>/` folder.
2. In Pactlab, **Start a Pact** with that currency as the base currency.
3. **Sources → Upload billing export → Pactlab standard template** → `invoice-lines.csv`.
4. **Documents** → upload the PDFs in `documents/`.
5. Work through the **planted findings** listed in that folder's README.

To adapt a pack to real data, keep the column headers and file layout and replace the values. Never commit real customer, employee or patient data to this repository.

## Licence

[CC0 1.0 Universal](LICENSE) — public-domain dedication. Use, change and share the data freely.
