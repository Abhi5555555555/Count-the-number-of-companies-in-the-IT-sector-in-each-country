# Count-the-number-of-companies-in-the-IT-sector-in-each-country
SQL
Count the number of companies in the Information Technology sector in each country.
Output the result along with the corresponding country name.
Order the result based on the number of companies in the descending order.

Table: forbes_global_2010_2014
Approach Hints
Expected Output
forbes_global_2010_2014
Preview
company:
varchar
sector:
varchar
industry:
varchar
continent:
varchar
country:
varchar
marketvalue:
float
sales:
float
profits:
float
assets:
float
rank:
int
forbeswebpage:
varchar


ans:
SELECT COUNT(company), country
FROM forbes_global_2010_2014
WHERE sector = 'Information Technology'
GROUP BY country
