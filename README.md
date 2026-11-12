---
language:
- en
license: other
license_name: shortlist-sg-compilation-terms
license_link: LICENSE.txt
task_categories:
- tabular-regression
tags:
- singapore
- business-software
- grants
- software-pricing
- edge-grant
size_categories:
- n<1K
configs:
- config_name: listings
  data_files:
  - split: train
    path: software-listings.csv
---

# Singapore EDGE Software Grants and Vendor Prices — November 2026

An independent, dated reference snapshot compiled by **Shortlist SG** for software-budget comparisons and reproducible analysis. This is **not an official dataset, an exhaustive directory, or an eligibility decision**.

## Original reference pages

- [EDGE qualifying cost caps by category](https://shortlistsg.com/edge-grant/caps)
- [Microsoft Dynamics 365 Business Central reseller comparison](https://shortlistsg.com/erp/microsoft-dynamics-365-singapore)
- [Shortlist SG](https://shortlistsg.com/)

Snapshot date: **12 November 2026**. Publisher: Shortlist SG. Contact: hello@shortlistsg.com. The site offers vendor quote requests and discloses its commercial model; it is not affiliated with Enterprise Singapore, IMDA, Microsoft or the listed vendors.

## Files and coverage

- `software-listings.csv`: 140 checked solution/vendor observations across 9 directory-category labels, copied unchanged from the project's dated CSV. One row is one solution/vendor observation with a listed starting price, not every available package.
- `category-caps.json`: the site's category reference, including qualifying cost caps where confirmed. Missing caps remain null; no cap is inferred for a different category.
- `dynamics-365-resellers.json`: six Business Central observations selected from the same listings snapshot.
- `metadata.json`: counts, source URLs, snapshot date and SHA-256 checksums.
- `LICENSE.txt`: reuse terms distinguishing original compilation contributions from third-party source rights.

## Field dictionary: software-listings.csv

| Field | Meaning |
| --- | --- |
| category | Checked directory-category label; some product families span several categories. |
| official_category_url | Official directory category used as the source. |
| product | Listed solution/product name; not a recommendation. |
| vendor | Listed vendor business name. |
| official_reviews | Directory review count in the dated snapshot; blank means unavailable. |
| starting_price_sgd | Listed starting package price in Singapore dollars before GST; not a personalised quotation. |
| estimated_grant_sgd | Shortlist SG estimate recorded in the source CSV; not an awarded or guaranteed grant. |
| verified_on | Date recorded by the project for the source check, in YYYY-MM-DD format. |

`category-caps.json` separates the **qualifying cost cap** from the indicative maximum support obtained by applying an SME or non-SME percentage. Actual support is subject to qualifying costs, eligibility, the applicable activity, annual limits and approval. Null means unconfirmed, not zero.

## Method and limitations

The project manually checked the official SMEs Go Digital directory and Enterprise Singapore activity pages, then arranged selected factual fields into a comparison reference. The CSV's `verified_on` field records that check; this release packages that snapshot and does not claim an additional independent audit of every official entry at publication time. Official URLs accompany the data so readers can check current requirements.

The six Business Central starting prices range from **S$8,530 to S$24,400** in this snapshot. Packages differ in licences, modules, implementation, migration and training. The range is **not** a like-for-like price comparison and does not prove that one vendor overcharges. It also does not claim these are every reseller in Singapore or every official category.

Estimated support is not equivalent to a discount already received. GST, maintenance, subscription duration, implementation details and qualifying cost definitions must be checked against the relevant official activity and quotation. Directory review counts are a dated observation, not a quality score assigned by Shortlist SG.

The data can become outdated. No automatic update schedule is promised. For current decisions, use official activity requirements, the live directory, a written vendor quotation and the Letter of Offer. This release contains no customer records, private contacts, logos, copied reviews, vendor descriptions or source-page prose.

## Sources and rights

- [Enterprise Singapore EDGE activity pages](https://www.enterprisesg.gov.sg/financial-support/edge-grant/automation-and-digitalisation/single-function-solutions)
- [IMDA SMEs Go Digital directory](https://smesgodigital.gov.sg/web/)
- [Enterprise Singapore terms](https://www.enterprisesg.gov.sg/terms-of-use)

Read `LICENSE.txt` before reuse. The custom license covers only rights the publisher holds in its original compilation, documentation and calculations. It does not relicense government material, vendor marks or other third-party content, or represent that those sources are CC0/open-licensed.

## Suggested citation

Shortlist SG (2026). *Singapore EDGE Software Grants and Vendor Prices — November 2026*. Snapshot dated 2026-11-12. Original reference: https://shortlistsg.com/edge-grant/caps . Identify the version and access date when citing; link readers to the relevant original comparison page and official source.

For corrections, provide the affected row, official source URL and the replacement value to hello@shortlistsg.com.
