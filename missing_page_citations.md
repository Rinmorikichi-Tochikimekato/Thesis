# Missing Page Numbers — Chapter 5 Citations (RESOLVED)

**Status: resolved.** All 13 PDFs turned out to already be in `Citations folder/`. All 29 citation
instances now have real page numbers (see commit `bd7b6b0`). In the process, ~12 claims were found
to be misattributed or unsupported by the source they cited — those were reworded and marked as
this report's own reasoning rather than a cited finding, rather than assigning a fabricated page.
Keeping this file for the record of what the original gap was.

These 13 sources are cited 29 times in Chapter 5 (advertiser/subscription/commercial-viability
content) without page numbers, because the source PDFs weren't available when the citations
were added. Pull each PDF via its DOI link, find the page(s) supporting the specific claim(s)
cited in `main.tex`, and send back the page number(s) per key (e.g. `2855351 -> p.12`).

| Key | Author(s) | Year | Title | DOI |
|---|---|---|---|---|
| 2855351 | Cao, Mingxuan | 2026 | Bridging Information Asymmetry through AI-driven FinTech: The Role of Digital Footprint Analytics in Financial Inclusion | https://doi.org/10.22158/ibes.v8n1p59 |
| 2977039 | Kostenko, Oleksii | 2025 | AI Law Model for Ethical Legislation: Strategic Recommendations for the Regulation of Artificial Intelligence | https://doi.org/10.69635/978-1-0690482-5-7 |
| 3303310 | Hu, Ziye | 2025 | Research on the Impact of Social Media Algorithmic on User Decision-making: Focus on Algorithmic Transparent and Ethical Design | https://doi.org/10.54254/2755-2721/2025.po24665 |
| 5142478 | Mariia, Gerr | 2025 | AI-Driven Content Curation and Its Impact on Media Diversity in Social Networks | https://doi.org/10.33422/worldcmc.v2i1.1050 |
| 5345089 | Mökander, Jakob | 2023 | Auditing of AI: Legal, Ethical and Technical Approaches | https://doi.org/10.1007/s44206-023-00074-y |
| 6087241 | Liu, Shimu & Keshavarz, Ashkan Lucas | 2026 | Dark Commercial Patterns and Consumer Behavior: A Conceptual Framework of Manipulation, Autonomy, and Trust | https://doi.org/10.32996/jpbs.2026.6.2.3 |
| 6295677 | Khare, Ankit; Khare, Prakriti; Siddha, Nisha | 2026 | Dark Patterns in Indian E-Commerce: Consumer Protection Challenges and Regulatory Gaps | https://doi.org/10.61877/ijmrp.v4i7.327 |
| 6454369 | Adako, O.P.; Adeusi, O.C.; Alaba, P.A. | 2024 | Revolutionizing Autism Education: Harnessing AI for Tailored Skill Development in Social, Emotional, and Independent Learning Domains | https://doi.org/10.47852/bonviewjcce42023414 |
| 6502223 | Chitra B, T.; Koushik Nayaka, U.; Mayur Kiran Kumar, S.; Sushanth, N.T. | 2026 | AI Recommendation Algorithms and Democratic Polarization: A Comprehensive Analysis of Algorithmic Influence on Public Opinion, Electoral Integrity, and Digital Constitutionalism | https://doi.org/10.22214/ijraset.2026.83777 |
| 7461574 | Bahangulu, Julien Kiesse; Owusu-Berko, Louis | 2025 | Algorithmic bias, data ethics, and governance: Ensuring fairness, transparency and compliance in AI-powered business analytics applications | https://doi.org/10.30574/wjarr.2025.25.2.0571 |
| 7646767 | Zhang, YuTian; Liu, YunHan | 2026 | Algorithms as Agenda Setters: The Case of Weibo's Zhisou AI and Its Ethical Implications in China's Media Ecology | https://doi.org/10.61784/tsshr3243 |
| 7896734 | Sanikidze, Sergo | 2026 | Dark Patterns in the Age of Artificial Intelligence: How AI Misleads Consumers in Global E-Commerce | https://doi.org/10.15837/aijes.v20i1.7638 |
| 8958037 | Li, Dan | 2026 | Psychological Mechanisms and Intervention Strategies for College Students' Short-Video Addiction in Algorithmic Recommendation Scenarios | https://doi.org/10.63313/esw.2014 |

## Where these are cited in `main.tex`

Line numbers as of the current file (Chapter 5, advertiser/subscription/commercial-viability subsections):

- Line 247: `7646767`
- Line 715: `6295677`
- Line 717: `6087241`, `6295677`
- Line 719: `5142478`, `6502223`
- Line 721: `6087241`, `6295677`, `6502223`, `5142478`
- Line 730: `7461574`, `8958037`, `6454369`, `2855351`
- Line 734: `3303310`, `5142478`
- Line 736: `7896734`, `6295677`, `3303310`, `5142478`, `2977039`
- Line 738: `6502223`, `3303310`, `7896734`
- Line 740: `6502223`, `2977039`, `3303310`, `5345089`, `7896734`

## How to send back page numbers

Once you have the PDFs, reply with something like:

```
2855351 -> p.12
2977039 -> p.4
3303310 -> p.7, p.9 (two different claims)
```

and I'll patch the `\parencites{}` calls in `main.tex` to `\parencites[page]{key}` accordingly.
