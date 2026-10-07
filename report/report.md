# Which Customers Should Get the Marketing Budget?

Customer groups from two years of online sales, December 2009 to December 2011

Gilbert Owen, portfolio project, October 2026

## 1. Executive Summary

This report helps an online gift retailer decide which customers to spend the marketing budget on, and how to treat each group of customers differently. The goal is to keep the high-value customers and win back the ones who are slipping away.

We used two years of sales from a UK online gift shop. We described every customer by how recently they bought, how often, and how much they spent, and put similar customers in the same group. This gave four groups.

The money is very concentrated. About 1 in 5 customers are Best Customers, and they bring 73.7% of the revenue. About 1 in 4 are Slipping Regulars, who ordered several times before, but the typical one has not ordered for 184 days. Together these two groups bring 90.1% of the revenue (£12.37M and £2.75M over the two years). The other two groups, Active Small Buyers and Lost One-timers, are more than half of the customers but bring less than 10%. All group numbers are for the 5,852 customers who have a customer ID.

By that, we should spend most of the budget on keeping the Best Customers happy and winning back the Slipping Regulars around August, before the September to November peak. Active Small Buyers only need cheap nudges to order more, and Lost One-timers get one automatic email, then no more budget. This protects most of the revenue and stops spending on customers who bring very little.

[ILLUSTRATION: four groups at a glance (figures/01-four-groups-at-a-glance.png)]

*Figure 1. The two groups at the top bring 90.1% of the revenue, so they get most of the budget.*

## 2. The Data We Used

The data is the Online Retail II dataset: 1,067,371 invoice lines from a UK online gift shop, from 1 December 2009 to 9 December 2011. We took out the lines that are not real product sales: cancellations (they are refunds, not purchases), postage, fees and adjustment lines, 33,757 duplicate lines, and three big orders that were cancelled right after they were placed. This leaves 1,003,354 clean sales lines.

About 23% of these lines have no customer ID. They are still real sales, so we keep them for the sales trends, but the customer groups can only use the 5,852 customers we can identify.

For spend, we count what customers bought before refunds. The cancelled big orders are already removed, so taking their refunds away again would count them twice. Our top spenders also return 5% or less of what they buy, so this choice doesn't make anyone look bigger than they are.

[ILLUSTRATION: from sales lines to four groups (figures/02-from-sales-lines-to-groups.png)]

*Figure 2. From 1,067,371 invoice lines we end with 5,852 customers in four groups, each described by the same three questions.*

## 3. What the Data Shows

### Sales peak in autumn, mostly because more customers buy

Both years have the same pattern: fairly flat from January to August, then sales rise from September and peak in November, at about £1.43M in 2010 and about £1.45M in 2011. From January to November, 2011 is flat against 2010 (revenue up 1.7%, orders down 3.7%). The autumn rise comes mostly from more customers buying, not from customers spending more. Customers per month go from about 750 in February to about 1,600 in November, while revenue per customer only moves between about £530 and £760.

By that, we should have stock and campaigns ready by August.

[CHART: revenue per month (figures/03-revenue-per-month.png)]

*Figure 3. November is the top month in both years, and the grey December 2011 bar is low only because the data stops on 9 December.*

### Most buyers come back, but fewer new customers join

From January to November 2011, nearly 9 in 10 buyers each month were returning customers (about 87%, up from about 77% in April to November 2010). But fewer new customers join: about 263 a month in April to November 2010, and only about 142 in the same months of 2011. Also, 27.7% of customers (1,619 of 5,852) ordered only once. Some of them first bought in late 2011 and had little time to come back, so the real share is a bit lower.

By that, we should follow up with every first-time buyer and run new-customer campaigns before the autumn peak.

[CHART: new vs returning customers per month (figures/04-new-vs-returning.png)]

*Figure 4. New customers (the dark part of each bar) fell from 375 in October 2010 to 221 in October 2011, and the shaded months are not used.*

### A small group of customers brings most of the money

Spend is very uneven. The average customer spent £2,868, but the typical customer only £856, because a few very big customers pull the average up. Only 4.6% of customers, fewer than 1 in 20, bring half of the revenue, and 23.5% bring 80%. The top 10 customers alone bring about 16%.

By that, we should keep our top customers happy first, for example with a personal contact and priority service.

[CHART: revenue concentration curve (figures/05-revenue-concentration.png)]

*Figure 5. Instead of following the grey line of equal spending, the curve shoots up: the first 4.6% of customers already bring half of the revenue.*

### After 150 days without buying, a customer is slipping away

To decide when a customer is "slipping away", we looked at how long customers wait between visits. Half of the return visits happen within 32 days, 3 in 4 within 70 days, and 9 in 10 within 148 days. So a customer who has not bought for 150 days is already later than 9 in 10 return visits, and that is our cutoff. By this rule, 43.8% of customers are slipping away, and a quarter have not bought for more than a year.

By that, we should send a win-back offer when a customer passes 150 days, or sooner for customers who usually buy every month.

[ILLUSTRATION: when a customer starts slipping away (figures/06-when-customers-slip.png)]

*Figure 6. The typical Slipping Regular (184 days) and Lost One-timer (401 days) are already past the 150-day line, while Best Customers and Active Small Buyers bought recently.*

### The UK is most of the business, but international buyers order bigger

The UK brings 85.3% of all revenue, and no other country brings more than 3.2%. But international customers place bigger orders: £859.8 on average, about 2 times the UK's £419.8, and they order just as often (6.2 vs 6.3 orders per customer). We kept all countries in the same groups, because the groups are about how people buy, not where they live, and only 7 countries outside the UK have 20 or more customers.

By that, we should keep the UK as the main market, but also take care of the few big international buyers.

[CHART: countries and order size (figures/07-countries.png)]

*Figure 7. The UK is by far the biggest market, but an international order is about twice the size of a UK order.*

### Returns are low, but a few products come back a lot

Only 2.4% of revenue is returned, and most months stay at about 1% to 2.5%. But for Black Cherry Lights, 99.5% of the sold value came back, and the other cherry lights, the willow branch lights and the pantry chopping board are also very high. This looks like a real problem with quality, damage or the product description.

By that, we should check the cherry lights and the chopping board first.

[CHART: products returned the most (figures/08-high-return-products.png)]

*Figure 8. Across all products only 2.4% of the sold value comes back, but for these five products it is between 46.9% and 99.5%.*

## 4. Four Groups of Customers

To build the groups, we described every customer with three numbers: days since the last order, number of orders, and total spend. This is called RFM (Recency, Frequency, Monetary). Then we used K-Means, a common method that puts customers with similar numbers into the same group.

We tried from 2 to 8 groups. Two groups only split active and inactive customers, which is too simple for marketing. Four groups gave the clearest split after that, and more groups did not make the customers inside each group much more alike. Four groups also means four clear plans, which a marketing team can manage.

To check the groups, we also sorted customers with simple hand-written rules, like "bought recently, often and a lot" or "no order for more than 150 days". The two ways mostly agree: 82% of the top customers by the rules are in Best Customers, 77% of the at-risk ones are in Slipping Regulars, and 97% of the lost ones are in Lost One-timers.

[CHART: share of customers vs share of revenue per group (figures/09-group-shares.png)]

*Figure 9. Best Customers are 20.3% of the customers but bring 73.7% of the revenue, while Lost One-timers are the biggest group (33.5%) but bring only 3.7%.*

## 5. What We Should Do With Each Group

The budget should not be spread equally, because each group needs something different:

- Best Customers: keep them happy first, with a personal contact, priority service and early access to new stock before the September to November peak. They already buy often, so they don't need big discounts.
- Slipping Regulars: win them back before they become lost. Send a reminder or a personal offer once a customer passes 150 days without buying (or 2 times their own usual gap), around August, before the autumn peak.
- Active Small Buyers: grow their orders with bundles and free postage above a minimum order, and follow up after the first order so they become regulars.
- Lost One-timers: one cheap automatic win-back email. If they don't come back, no more budget.

Beside the groups, we should check the high-return products (the cherry lights and the pantry chopping board), and give the big international buyers the Best Customers treatment, because they make bigger orders.

For the possible business impact, we look at the money each group brings. Best Customers brought £12.37M in two years, so losing even a few of them hurts more than losing many small buyers. Slipping Regulars brought £2.75M, and most buyers in the autumn peak are returning customers, so every regular we win back before September can buy again in the busiest months. Lost One-timers are a third of the customers but brought only £0.62M, so stopping after one email saves budget with little risk.

By that, most of the budget should go to keeping the Best Customers and winning back the Slipping Regulars, because together they bring 90.1% of the revenue.

## 6. Reflection

We chose RFM with K-Means because it is simple, easy to explain to non-technical people, and answers which customers to spend the budget on. A few things went well: it only needs sales data the shop already has, every cleaning step is written down so anyone can repeat the numbers, and the groups mostly match the simple rules (82% of the top customers and 97% of the lost ones).

Some things are not good yet:

- About 23% of sales lines have no customer ID, so those buyers are not in any group.
- RFM only looks at the past and doesn't use products, country or returns, and the 150-day cutoff is the same for everyone.
- The groups overlap a bit at the edges, and their sizes can shift a little if the data is updated.
- The data starts in December 2009 and stops on 9 December 2011, so customers near the edges look newer or more slipping than they really are.

Next, we would like to:

- use each customer's own buying rhythm to decide when they are slipping
- add return rate, average order value and country, and compare with other grouping methods
- predict which customers are likely to stop buying, and how much each customer may be worth
- test the win-back email on a small group first, to measure the real effect

## 7. Use of Generative AI

We used Generative AI in these parts of the work:

- some help building the code
- help correcting the interpretations and the code
- drafting the summary points
- help converting the essential information from the notebook into this report, such as the visualisations

All numbers in this report come from the notebook outputs.
