# Mindfactory_GPU_Crawler
Script that automatically scrapes the Website of the german IT retailer "Mindfactory" to gather gaming grade GPU sales information.

EN
----------------------------------------
**Bottom Line**: Script that automatically parses Mindfactory's website top gather sales information on gaming grade gpus, processes this information and saves it as a pandas dataframe. This information can and will be used to publish monthly sales overviewes, as well as additonal further analysis.

**Background**: The gaming gpu market is mainly comprised of two rivaling companies, AMD and Nvidia. In the recent months the market for gpus has picked up some speed due to AMD's release of their new RDNA architecture gpus (RX 5700 & RX 5700 XT) and Nividas subsequent release of their "Super" gpus (2060 Super, 2070 Super, 2080 Super). As a consequence, this does only provide customers with additional purchase options, it also provides data analyst with the opportunity to track sales numbers from directly rivaling products "from day one", due to their almost simultaneous release dates.

**Functionality**

1. Output:

- GPU Name
- No of sold items at the given point in time
- Retail price at the given point in time
- Amount of VRAM
- GPU Model name
- GPU Architecture
- Timestamp (using the datetime format).

Creates one gpu_df file marked with a timestamp.

2. Input

- List of urls, organized by gpu model

3. Used modules

- request
- BeautifulSoup
- pandas
- datetime
- re

Inspired by the reddit user Ingebor's (https://www.reddit.com/user/ingebor) monthly cpu sales overwiev.

