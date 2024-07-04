# SHG-Booking-Data-Analysis
An analysis on the SHG booking data.
Objectives
The renowned hospitality company Splendour Hotel Group (SHG) aims to improve visitor experiences and streamline corporate processes by utilizing data-driven insights. By diving into the data, we aim to extract meaningful insights that will not only inform operational improvements but also contribute to SHG's overall success in delivering unparalleled hospitality.
Dataset
The dataset consists of 119,390 rows and 17 columns, containing the following information:
•	Booking ID: Unique identifier for each booking.
•	Hotel: Type or name of the hotel within the Splendour Hotel Group.
•	Booking Date: Date when the booking was made.
•	Arrival Date: Date when the guests are scheduled to arrive.
•	Lead Time: Number of days between the booking date and arrival date.
•	Nights: Number of nights the guests are booked to stay.
•	Guests: Number of guests included in the booking.
•	Distribution Channel: The channel through which the booking was made (e.g., Direct, Online Travel Agent, Offline Travel Agent).
•	Customer Type: Type of customer making the booking (e.g., Transient, Corporate).
•	Country: Country of origin of the guests.
•	Deposit Type: Whether a deposit was made for the booking (e.g., No Deposit, Deposit).
•	Avg Daily Rate: Average daily rate for the booking.
•	Status: Status of the booking (e.g., Check-Out, Cancelled).
•	Status Update: Date of the last status update for the booking.
•	Cancelled (0/1): Binary indicator of whether the booking was cancelled (1 if cancelled, 0 if not cancelled).
•	Revenue: Revenue generated from the booking.
•	Revenue Loss: Loss in revenue if the booking was cancelled (negative value if the booking wasn't cancelled).
Data Cleaning and Preparation
Once the data was downloaded and imported into Excel, it was cleaned and prepared for analysis. A copy of the original data was stored in Google Drive to allow for easy access. Firstly, a new version of the data was created in case there was a need to drop some columns or make other changes. In the newly created worksheet, the following steps were taken:
•	Missing values: A thorough check for blanks in all the columns was carried out. Missing values in the country column were replaced with ‘N/A’. The distribution channel column had five rows with missing values, which were replaced with the most frequent value.
•	Data types: All columns were in the format needed for analysis.
•	Outliers: The guests column had some outlier values, with as high as 55 guests per booking. Such values contributed to less than 1% of the dataset.
•	Categorical variables: These were examined for errors in spellings and other unexpected values. No errors were found.
•	Data extraction: For clearer analysis, the month and day of the week were extracted from the booking dates, arrival dates, and status update columns.
Data Exploration
With the data cleaned and ready for use, the next step was exploration and analysis. The exploratory data analysis started by looking into the booking patterns to identify seasons with noticeable booking activity and to examine the impact of booking channels and customer type on lead time. We also investigated customer behavior and revenue optimization to identify overall revenue trends, significant contributors to revenue, and the impact of average daily rates across booking channels.
Insights
Booking Patterns
•	There were a total of 119,390 bookings in the last five years, with 2016 having the highest number of bookings. A dip was seen in 2017, but this is inconclusive as the data for 2017 only covers eight months.
•	January and February saw the greatest number of bookings, which gradually dipped until June. There was no specific pattern until a noticeable increase in October, followed by a dip until December.
•	The first three months and the last three months of the year had the most bookings and the longest average lead times, suggesting these were premeditated trips targeting holidays in the summer seasons.
•	The lead time was highest on average among bookings made via Offline and Online Travel Agents at 136 days and 108 days respectively, and lowest for Corporate channels at 45 days. Contract customers had the most lead time averaging 143 days, while Groups had an average lead time of 55 days, suggesting that contract customers may take more time planning their stays than groups.
Customer Behavior Analysis
•	Online Travel Agents contributed to over half of the total bookings, with 74,000 bookings and the highest average daily rate at $109. Direct bookings had an average daily rate of $107 but accounted for just 15,000 bookings.
•	Portugal, the United Kingdom, and France were the top three countries of origin for customers. Portugal led with 49,000 bookings, contributing about $9.0M to revenue. The United Kingdom and France contributed $4.2M and $3.1M respectively, with 12,000 and 10,000 bookings each.
Revenue Optimization
•	The total revenue generated was $29.60M, with $9.0M from Portugal. Transient customers contributed $22.70M, over 75% of the total revenue, making them primary drivers.
•	By distribution channel, Online Travel Agents contributed $17.3M to the revenue, aligning with their high booking volume. The average daily rate was $109 for Online Travel Agents.
•	Transient customers had a higher average daily rate at $107, explaining their significant revenue contribution. Most bookings and revenue from Online Travel Agents were driven by Transient customers.
Cancellation Analysis
•	The total number of cancelled bookings was 44,224, with 1,207 no-shows.
•	Revenue lost from cancellations was $13.12M. Transient customers and Online Travel Agents, the biggest revenue drivers, also contributed significantly to cancellations and revenue loss.
Impact of Deposit Types
•	Transient customers contributed more to non-refundable deposits, hence the most to revenue from cancelled bookings.
•	More cancellations occurred where there was no deposit, representing about 24,000 of the total cancellations. The least cancellations were seen with refundable deposits, at just 36. Non-refundable deposits contributed $3.60M to the revenue, suggesting a potential area for optimization.
Operational Efficiency
•	A total of 234,988 guests were served, with an average stay of approximately three nights. Bookings made by Offline Travel Agents had an average stay of four nights, while Online Travel Agents had an average of three.
•	Contract customers averaged five nights per stay, while other customer types averaged three.
•	The average number of guests per booking was approximately two, making up 69% of the distribution. Large groups were rare outliers.
•	Online Travel Agents accounted for 65% of the total guests, while the corporate channel made up just 4%.
•	Fridays were the most popular arrival day, and most check-outs occurred on Sundays, indicating weekend stays are popular.
•	August had the most check-outs, suggesting the end of the summer season. This could advise more staffing and resource allocations during these periods for optimal efficiency.
Analysis of Corporate Bookings
•	Corporate bookings were the least in number and had the least average daily rate at $69. This is significantly lower than other channels like Online Travel Agents ($109) and Direct bookings ($107).
•	Corporate bookings had the shortest lead time at 45 days. Given the desirably short lead time, it would be wise to increase the average daily rate for this channel to generate more revenue.
Geographical Analysis
•	Most customers originated from Portugal, followed by the United Kingdom, France, Spain, and Germany. Portugal contributed 90,000 guests, while the United Kingdom, France, and Spain contributed 25,000, 22,000, and 18,000 guests respectively.
•	These countries were the greatest revenue contributors but also had high cancellation rates. Enforcing non-refundable deposits could help mitigate revenue loss from cancellations.
•	The average daily rate for these countries was typical, with Portugal having the lowest at $92. No definite pattern was observed between country of origin and the average number of nights spent.
Time-to-Event Analysis
•	Lead times were classified into two-month ranges to examine variations. Lead times between 0-2 months and 2-4 months were associated with the highest number of bookings and revenue. However, these lead times also had the highest cancellations and revenue loss, suggesting the relationships might be cause and effect rather than truly significant.
Comparison of Online and Offline Travel Agents
•	Online travel agents contributed the most bookings (74,000) and the most revenue ($17.3M), tripling the contributions of offline travel agents.
•	Online travel agents also had the highest cancellation rates, contributing to 72% of cancellations.
RECOMMENDATIONS
Marketing and Revenue Optimization:
•	Target peak seasons and top source countries: Focus marketing efforts on summer seasons and high-revenue generating countries like Portugal, UK, France, Spain, and Germany. Consider targeted campaigns and promotions to attract guests from these regions during peak booking times.
•	Review Corporate booking pricing: Corporate bookings have a short lead time (45 days) but a lower ADR ($69) compared to other channels. Analyze competitor pricing for similar corporate stays and consider raising SHG's corporate rates to potentially increase revenue without significantly impacting lead times.
•	Encourage non-refundable deposits: The data shows non-refundable deposits contribute significantly to revenue from cancellations ($3.60M). Explore offering incentives (discounts, upgrades) for guests who choose non-refundable deposits to potentially reduce cancellations and boost revenue.
Operational Efficiency:
•	Optimize staffing and resources: Allocate staffing and resources strategically based on booking patterns. Focus on having adequate personnel during peak seasons (summer months, weekends) and consider flexible scheduling to accommodate high arrival and check-out days (Fridays & Sundays).
•	Upselling and cross-selling opportunities: Analyze guest profiles and booking types to identify upselling and cross-selling opportunities. For example, offer room upgrades or spa treatments to guests with a higher ADR or longer stays.
Cancellation Management:
•	Implement Non-Refundable Deposits: Since cancellations lead to substantial revenue loss, incentivize guests to opt for non-refundable deposits. This strategy can reduce cancellations and secure revenue even when bookings are cancelled.
•	Enhance Communication on Deposit Policies: Clearly communicate deposit policies during the booking process to manage guest expectations and reduce last-minute cancellations.
Continuous Data Monitoring:
•	Implement regular data analysis and monitoring to capture evolving booking patterns, customer preferences, and market trends. This proactive approach will facilitate timely adjustments in strategies and operations.
