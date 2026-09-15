1. At what array size did your baseline algorithm become noticeably sluggish to execute?

My array had a noticeable slowdown that I could feel at 5,000 upwards and any higher it gets impossible to miss.

2. Based on your empirical data and the shape of your graph, estimate how long (in seconds, minutes, or hours) your baseline algorithm would take to process an array of $1,000,000$ elements. Show your reasoning.

Since this algorithm is O(n²), the time grows with the square of the size. So if we go from 10,000 numbers up to 1,000,000 numbers, that's 100 times bigger — but the time grows by 100², which is 10,000 times longer.
time(1,000,000) ≈ time(10,000) × (1,000,000 / 10,000)²
≈ 2.454237 s × 100²
≈ 24,542 seconds
≈ 409 minutes
≈ ~6.8 hours

3. Based on your empirical data and the shape of your graph, estimate how long (in seconds, minutes, or hours) your Kadane's algorithm would take to process an array of $1,000,000$ elements. Show your reasoning.

Kadane's is O(n), so the time just grows in a straight line with the size — no squaring. Going from 10,000 to 1,000,000 numbers is 100 times bigger, so it just takes 100 times longer.
0.000433 seconds × 100 ≈ 0.043 seconds