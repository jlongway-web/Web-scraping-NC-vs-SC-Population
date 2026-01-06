### NC vs SC population growth
A web scraping project comparing population grown in North and South Carolina
* Wikipedia was selected due to its scraping policy and data availability

While this project leverages the foundational scraping techniques from the IBM Data Science Professional Certificate, it extends the scope by performing multi-source data merging and implementing a custom cleaning pipeline to handle real-world Wikipedia HTML inconsistencies.

🛠️ Tools Used: 
* Data Handling: Pandas, NumPy
* Web Scraping: BeautifulSoup4, Requests
* Visualization: Seaborn, Matplotlib

🚩 Technical Challenges:
* Non-numeric Characters - Implemented Regex (\D) to strip Wikipedia citation brackets (e.g., [1]) from years and populations.
* Inconsistent Dash Types - Identified and handled the dash (—) in the first row of census data to prevent float conversion errors.
* Idempotent Pipeline - Built a cleaning function that checks dtypes before processing, allowing the notebook to be re-run without errors.


![](images/nc_sc_population_growth.png)
💡 Key Insight: The 1970 divergence coincides with the "Sun Belt" migration and the maturation of the Research Triangle Park in NC. While SC maintained a steady growth through manufacturing, NC's pivot toward high-growth finance (Charlotte) and tech (Raleigh) sectors created an exponential population trajectory.
