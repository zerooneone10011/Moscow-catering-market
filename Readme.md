<b>Research task</b><p>
Prepare a study of the Moscow catering market, find interesting features that will help in the future in choosing a suitable place to open a new establishment.
<p>
A dataset with catering establishments in Moscow is available, compiled on the basis of data from Yandex Maps and Yandex Business services for the summer of 2022. The information posted in the Yandex Business service could have been added by users or found in publicly available sources. It is for reference only.

<b>Description of data</b><p>
File moscow_places.csv:<p>
name - the name of the institution;<p>
address - the address of the institution;<p>
category - the category of the establishment, for example, "cafe", "pizzeria" or "coffee shop";<p>
hours - information about the days and hours of work;<p>
lat is the latitude of the geographic point where the establishment is located;<p>
lng - longitude of the geographic point where the institution is located;<p>
rating — institution rating according to user ratings in Yandex Maps (highest rating — 5.0);<p>
price — category of prices in the institution, for example, “average”, “below average”, “above average”, and so on;<p>
avg_bill is a string that stores the average cost of an order as a range, for example:<p>
“Average bill: 1000–1500 ₽”;<p>
“Price of a cup of cappuccino: 130–220 ₽”;<p>
“The price of a glass of beer: 400–600 ₽.”<p>
and so on;<p>
middle_avg_bill is a number with an estimate of the average bill, which is indicated only for values from the avg_bill column that begin with the "Average bill" substring:<p>
If a row contains a price range of two values, the column will contain the median of the two values.<p>
If the line contains one number — the price without a range, then this number will be included in the column.<p><p>
If there is no value or it does not start with the substring "Average score", then nothing will enter the column.<p>
middle_coffee_cup is a number with an estimate of one cup of cappuccino, which is indicated only for values from the avg_bill column that begin with the substring "Price of one cup of cappuccino":<p>
If a row contains a price range of two values, the column will contain the median of the two values.<p>
If the line contains one number — the price without a range, then this number will be included in the column.<p>
If there is no value or it does not start with the substring "Price of one cup of cappuccino", then nothing will be included in the column.<p>
chain — a number, expressed as 0 or 1, that indicates whether the establishment is a chain establishment (errors may occur for small chains):<p>
0 - the institution is not a network<p>
1 - the institution is a network<p>
district - the administrative district in which the institution is located, for example, the Central Administrative District;<p>
seats — number of seats.
