Mini-project showing SQL + Python analysis on a transactions dataset.
Notebook uses DuckDB (SQL on CSV), pandas, and matplotlib.
It calculates fraud rate overall and by channel, 3DS, AVS/CVV, distance, and country vs BIN country.
Includes 3 simple charts and a short summary of findings.
Dataset (`transactions.csv`) is not included.

Across 299,695 transactions, overall fraud rate is approx 2.21%. Fraud is concentrated in web channel segment (approx 3.56%), approx 4× higher than app ( approx 0.80%) Non-3DS transactions (approx 6.75%) are approx 7× higher than 3DS (approx 0.96%). Shipping distance shows a significant increase for 500km+ deliveries (approx 15.9%). Fail/fail transactions show approx 20× higher fraud rate than pass/pass. Hour level anomaly scan highlights several time windows with elevated fraud rates.
