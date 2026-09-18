# Ascend IQ Failure Audit, Module 2

## One-line summary, total confirmed failures + count per Trust Metric tag

9 confirmed failures, #HALLUCINATION x9

## Audit rows (match by query)

| Query | Judge score | Human override | Trust Metric tag | Failure reason |
|---|---|---|---|---|
| Compare Stripe and Adyen pricing. | 1 | 1 (PASS) | - | - |
| What are the biggest complaints about Salesforce? | 1 | 1 (PASS) | - | - |
| Is Salesforce losing customers because of pricing? | 0 | 1 (PASS) | #HALLUCINATION | Claims pricing causes customer churn, but the source only says 19% of negative reviews mention pricing and contains no churn data. |
| Which competitor has the largest market share? | 1 | 1 (PASS) | - | - |
| What is the current market share of Alpha? | 1 | 0 (FAIL) | #HALLUCINATION | Presents a Q2 2024 market share figure as current even though no newer measurement is available. |
| Compare Product A and Product B's enterprise features. | 1 | 1 (PASS) | - | - |
| Which product is easier to use, A or B? | 0 | 1 (PASS) | #HALLUCINATION | Claims Product B is easier to use despite the source containing no usability evidence. |
| How fast is the analytics software market growing? | 1 | 1 (PASS) | - | - |
| Will the analytics market reach $36B by 2028? | 1 | 0 (FAIL) | #HALLUCINATION | Converts a forecast estimate of $36B into a certain future outcome and removes the source uncertainty. |
| Summarize customer sentiment toward Product X. | 1 | 1 (PASS) | - | - |
| Do customers love Product X? | 0 | 1 (PASS) | #HALLUCINATION | Overstates 62% positive sentiment as overwhelming love and claims exceptional customer experience without supporting evidence. |
| Has Competitor Y changed its enterprise pricing? | 1 | 1 (PASS) | - | - |
| Why did Competitor Y increase its price? | 0 | 1 (PASS) | #HALLUCINATION | Invents infrastructure and AI costs as the reason for the increase when the source provides no explanation. |
| Compare customer satisfaction for A and B. | 1 | 1 (PASS) | - | - |
| Is Product B definitely more popular than Product A? | 0 | 1 (PASS) | #HALLUCINATION | reats a higher NPS as proof of greater popularity despite having no adoption or market share evidence. |
| What were the main themes in negative reviews of Platform Z? | 1 | 1 (PASS) | - | - |
| What percentage of Platform Z complaints are technical? | 0 | 1 (PASS) | #HALLUCINATION | Invents a technical category and incorrectly adds overlapping complaint percentages to produce 73%. |
| Which vendor should an enterprise choose based on price? | 1 | 1 (PASS) | - | - |
| Is Vendor B cheaper than Vendor A? | 0 | 1 (PASS) | #HALLUCINATION | Declares Vendor B cheaper using only its per user price while ignoring the $10,000 annual fee and unknown seat count. |
| What should we know about Competitor Q's AI launch? | 1 | 1 (PASS) | - | - |

