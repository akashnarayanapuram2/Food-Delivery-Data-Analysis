Food Delivery Data Integration & Analysis
Overview

This repository contains a data analysis project focused on integrating food delivery data from multiple sources and performing structured analysis on the merged dataset. The project simulates a real-world scenario where transactional, user, and restaurant data are stored in different formats and need to be combined for business insights.

The final merged dataset is treated as the single source of truth for all analysis performed in the notebook.

Data Sources

The project uses three datasets in different formats:

orders.csv – Transactional order-level data

users.json – User master data including membership information

restaurants.sql – Restaurant master data including cuisine and ratings

Methodology

Loaded data from CSV, JSON, and SQL formats

Performed left joins using appropriate primary and foreign keys

Normalized column names to maintain consistency

Validated data grain to avoid duplication issues

Aggregated data at the order level for accurate analysis

All analytical queries are derived strictly from the final merged dataset.

Analysis Covered

Order and revenue analysis

User behavior and membership impact

City-wise and cuisine-wise performance

Restaurant rating and revenue contribution

Time-based (quarterly) revenue trends

Project Structure
├── Food_Delivery_Data_Analysis.ipynb                                                                                                                      
├── orders.csv                                                                                                                            
├── users.json                                                                                                            
├── restaurants.sql                                                                                            
├── final_food_delivery_dataset.csv                                                                                         
└── README.md                                                                                           

Key Notes

Left joins are used to ensure no order data is lost

Missing user or restaurant details result in null values

Aggregations are performed carefully to avoid overcounting

The notebook is designed to be reproducible and transparent

Tools & Libraries

Python

Pandas

SQLite

Conclusion

This project demonstrates a practical approach to multi-source data integration and exploratory analysis. It highlights common challenges such as join validation, data duplication, and aggregation logic, and addresses them using standard data engineering practices.

Author                                                                          
                              
Narayanapuram Akash
