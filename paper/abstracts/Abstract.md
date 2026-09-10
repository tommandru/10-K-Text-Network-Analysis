## Abstract - CompleNet 2026

---
tags:
  - project/10KNetwork
  - type/reading
---

This research explores if transitions in company's product and business mix across the years can predict a company's future; To extract the products and service segments we use the annual reports companies file with securities and exchange commission (SEC) also known as 10-K. 10-Ks provide a rich information on company's businesses/products, risks, financial condition and company from the view of management. We aim to extract the business/products from Item1, Risks from Item 1A , Management's discussion and views from Item 7 and quantitative risks to the company's margins from Item 7A and all financial statements (Cash flow, Income and Balance sheet) from Item 8.  All the data points can be used build a network of products/businesses for each company; An accompanying the network of risks from Item 1A;  Financial Network and View Network and observe the temporal changes. This multilayer network can be used for link prediction - For example, if a company's node position in the _Risk Layer_ begins heavily clustering near failing companies, but its _Product Layer_ still looks healthy, your model can predict an impending downturn before it hits Item 8 (Financials). Another idea is trying to identify "structural signatures" of companies right before they undergo major transitions (e.g., how Netflix shifted from DVD shipping to streaming).  The network also allows us to find communities of companies that cluster across layers (e.g., they share the same risks _and_ the same product space) and track how these communities merge, split, or dissolve over the years. 


***Data Gathering and Extraction:***
- Data gathering part of work entails getting the annual reports from  securities and exchange commission (SEC)
- Once the data is gathered; Automated scripts extract the relevant parts of reports - Item 1 (Business), Item 1A (Risks), Item 7(Management Discussion), Item 7A (Quantitative Risks) and Item 8 (Financial Statements)
***Topic Modeling:***
- Develop efficient method to map similar products and segments as one topic; For example META describes(Facebook, WhatsApp and Instagram) as Family of Apps and their key revenue source is advertising, similarly Alphabet as diverse media platforms and their revenue is advertisements and Reddit is another example, the firm describes itself as collection of global digital communities but major revenue source is advertisements. The key challenge is to map all three items as one key word for comparison
