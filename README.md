# [Point Connect Data Retrieval via RDMS API](https://developers.refinitiv.com/en/article-catalog/article/point-connect-data-retrieval-via-rdms-api)

- You can check the code to retrieve temperature curve data with other RDMS endpoints in file rdms-pointconnect-temperature.ipynb in this GitHub repository.
- Retrieve data of multiple curves, merge them together using value_date, and convert to pandas dataframe.

Every day, we are faced with monumental amounts of data and content from every single direction. This includes everything from articles, posts, tweets, and emails flowing into our inboxes to the hundreds of ever-changing fundamentals around the global commodities complex. With Refinitiv Data Management Solution (RDMS) We enable you to make the best possible use of your data, technology, and human or artificial intelligence. We provide you with access to the most comprehensive, trusted, and up-to-date data on the global commodity markets. Our integrated solution ensures consumption of big data in a logical and structured manner, to extract maximum value from your internal or external data sets at a lower cost.

This article provides a guide to retrieving the commodities Point Connect data via RDMS API using Python programming language (as this is the REST API, any programming language that supports it can be used to make an API call) by demonstrating how to retrieve the temperature data and transforming the JSON responses into a dataframe for further steps such as visualizations or analytics, etc.

## Introduction
![image](https://github.com/Refinitiv-API-Samples/Article.RDMS.Python.RetrievePointConnectData/assets/89068039/22384c5f-2fa6-4091-882e-c0974228e498)
 - [Refinitiv Data Management Solution (RDMS)](https://www.refinitiv.com/en/trading-solutions/commodities-trading/data-management-solutions-commodities-trading) is the Cloud-based or in-house infrastructure for streamlined data warehousing
This comprehensive solution comes with the added option of accessing all the information via our platforms or integrating it with in-house visualization or data management systems via an open API framework. This reduces the total cost of ownership (TCO) at your end. This is the most effective solution for companies with exposure to commodities, including Energy companies, Utilities companies, Mining and materials companies, Agriculture and F&B companies, Transportation companies and airlines, and Commodities trading houses.
    - For RDMS API Overview, Quickstart, and Documentation can be found in the [Developer Portal - RDMS](https://developers.refinitiv.com/en/api-catalog/rdms/rdms)
 - [Refinitiv Point Connect](https://www.refinitiv.com/en/trading-solutions/commodities-trading/point-connect) is one of the sources of data that aggregated, normalized along with data from other sources, which can be retrieved using RDMS API
With Refinitiv® Point Connect, you can view fundamental and forecast data for power, gas, agriculture, weather, hydrology, carbon, liquefied natural gas (LNG), and metals. Gain insight from the Refinitiv Research and Forecasts team. See a full history of all data sets, with data delivery over FTP. Receive instant notifications on updated data with your subscription. Point Connect presents data simply in CSV files – and all in our metadata taxonomy for immediate access and context.

## Prerequisite
This example requires the below, or you can connect your Refinitiv account representative for further information.

1. For permission to access **Point Connect** data, more detail can be found [here](https://www.refinitiv.com/en/trading-solutions/commodities-trading/point-connect).
2. **Refinitiv Data Management Solutions (RDMS)**, more detail can be found [here](https://www.refinitiv.com/en/trading-solutions/commodities-trading/data-management-solutions-commodities-trading). You will get an account to access the specific instance of RDMS that contains the data set that you're interested in. It's recommended to follow the [RDMS REST API Quick Start Guide](https://developers.refinitiv.com/en/api-catalog/rdms/rdms/quickstart) to do the User Setup, Registration, Manage your account, Access the RDMS Administrator Web Application, and Access the RDMS Swagger REST API Page.
The guide to generating the RDMS API key, which is required for accessing data via RDMS API, is also provided in the quick start guide.
3. You also need an internet connection to connect to RDMS.
4. The tool for an API call, here we're using Python version 3.9.12 with these Python libraries
    - requests==2.27.1
    - pandas==1.3.5

## Conclusion
Our exploration of the RDMS API and Point Connect has demonstrated the immense potential of commodities data, specifically temperature data, for a wide range of applications. By learning to retrieve and transform this data into a dataframe format, you've gained a powerful tool for further analysis, and visualizations, and also easy to read by humans.

While this article demonstrated how to get temperature data, the skills you've acquired here can be applied to various other data types. So, whether you're a data scientist, financial analyst, or data enthusiast, the possibilities are now here for you to further explore and harness the power of commodities data. The journey doesn't end here, keep experimenting, keep analyzing, and keep discovering new insights! and if you have any questions regarding our API usage, feel free to check our Q&A forum or post the question there to get in touch. For questions related to the product or content, please raise a ticket via MyRefinitiv and the support team is going to reach out to you to assist with this. I hope you find this article helpful and please let me know if you have any use case you're interested to see its related article or code example.

### Reference
- [Dev Portal - Refinitiv Data Management Solution (RDMS)](https://developers.refinitiv.com/en/api-catalog/rdms/rdms)
   - RDMS Web Application: https://your-rdms-instance.rdms.refinitiv.com/
   - Generate API key: https://your-rdms-instance.rdms.refinitiv.com/Identity/Account/Manage/ApiKeys
   - RDMS swagger: https://your-rdms-instance.rdms.refinitiv.com/api/swagger/index.html
- [Q&A forum](https://community.developers.refinitiv.com/index.html)
   - [RDMS tag](https://community.developers.refinitiv.com/tags/56131/rdms.html)
