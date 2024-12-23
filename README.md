# HackerRank-SQL-Basic-Test

Student analysis SQL solution-

SELECT s.roll_number,s.name
FROM student_information s
INNER JOIN examination_marks e
ON s.roll_number = e.roll_number
GROUP BY e.roll_number
HAVING SUM(e.subject_one + e.subject_two + e.subject_three) < 100;

Profitable Stocks - 

SELECT a.stock_code
FROM price_today a
INNER JOIN price_tomorrow b
ON a.stock_code = b.stock_code
WHERE b.price>a.price
ORDER BY stock_code asc;

