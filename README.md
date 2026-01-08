# Email-Analytics
## Business need
Collect data that will help analyze account creation dynamics, user activity by email (sending, opening, clicks), and evaluate behavior in categories such as sending interval, account verification, and subscription status. The data should allow for comparing activity between countries, identifying key markets, and segmenting users according to various parameters.
## Solution
Write an SQL query in BigQuery to collect the necessary data.
#### List of output categorical values:
- date — date (for accounts — account creation date, for emails — email sending date);
- country — country;
- send_interval — sending interval set by the account;
- is_verified — whether the account is verified or not;
- is_unsubscribed — whether the subscriber has unsubscribed or not.
#### List of key metrics:
- account_cnt — number of accounts created;
- sent_msg — number of messages sent;
- open_msg — number of messages opened;
- visit_msg — number of clicks on messages.
#### List of additional metrics:
- total_country_account_cnt — total number of subscribers created in the country as a whole;
- total_country_sent_cnt — total number of letters sent in the country as a whole;
- rank_total_country_account_cnt — ranking of countries by the number of subscribers created in the country as a whole;
- rank_total_country_sent_cnt — ranking of countries by the number of letters sent in the country as a whole.
### Result of code execution

<img width="1047" height="570" alt="Знімок екрана 2026-01-08 о 17 03 36" src="https://github.com/user-attachments/assets/c7c6f1e1-5223-4887-b491-a787d04dc37c" />

### Visualizing results in Looker Studio

<img width="2500" height="2500" alt="Звіти_Looker_Studio_-_25 10 25,_07_38-1" src="https://github.com/user-attachments/assets/ff50ac47-432d-4ea5-97f8-8f85c69ef358" />
