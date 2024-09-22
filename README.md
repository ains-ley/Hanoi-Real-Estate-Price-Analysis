# Hanoi Real Estate Data Analysis (2019 -2023)

### Objective:
Conducted extensive data analysis and cleaning on a large dataset of real estate listings in Hanoi to explore patterns and derive insights into the market.

### Tools: 
Pandas, Seaborn, Matplotlib, Regular Expressions, Word Cloud

### Data Preparation:
1. Handling Missing Values: Identified and addressed missing values, outliers, and inconsistencies in key columns like "price" column.
2. Feature Extration: Developed custom logic using regular expressions to accurately extract district and ward information from the address column.
3. Text Normalization: A large amount of information in the listings is presented in text form. I cleaned and processed these text-based fields using Python and its libraries. The transformations applied include:
   * Normalizing Unicode to the NFC (Normalization Form C) format.
   * Standardizing the Vietnamese Unicode encoding to precomposed Unicode (NFC).

### Exploratory Data Analysis:
#### 1. Number of Estates in Hanoi:
   ![image](https://github.com/user-attachments/assets/4e700b2c-3c14-4266-bb64-4acbc13b8191)
- The central districts of the city have the highest number of real estate listings. This indicates that real estate transactions are more active in these areas compared to the outskirts. This is understandable as the city center, being the heart of the capital, hosts many businesses, services, and administrative offices, making it more attractive for real estate activities. Moreover, it is possible that real estate transactions in other areas are not frequently advertised on the websites I collected data from, and might instead be facilitated through different channels, such as private communication methods.
  
  ![image](https://github.com/user-attachments/assets/66a99409-e35c-4944-9ff9-33b5d08073ac)
- Examining real estate density by calculating the number of listings per unit area for each region. The real estate density map once again confirms that the city center is the most active area for real estate transactions.
  + The leading districts are Đống Đa, Thanh Xuân, Cầu Giấy, and Hai Bà Trưng.
  + Dịch Vọng has the highest number of real estate listings, while Bạch Mai has the highest density of real estate activity.

  ![image](https://github.com/user-attachments/assets/9e7dea9c-f8de-4c95-bebc-31e3b9bf0a60)
- Most of the listings consist of private houses, ranging from alleyways to main streets, as well as apartments. Additionally, there were some listings for land. It is evident that villas, which belong to a more premium segment, have fewer listings. Other real estate types being sold include properties that have been used for different functions such as offices, restaurants, shops, warehouses, etc. Since the dataset only covers real estate in Hanoi, properties used for agricultural or industrial purposes are relatively rare or almost non-existent.

  ![image](https://github.com/user-attachments/assets/45a404e7-c0cf-4712-86ea-aae152bd232e)
- Narrow alley houses ("nhà ngõ hẻm") and street-facing houses ("nhà mặt tiền") constitute the majority of real estate listings in Hanoi, especially in the inner-city districts. In these listings, there is typically a balanced distribution between alley houses and main street houses, or a greater prevalence of main street houses.
  + In Hoàn Kiếm district, the majority of properties listed are main street houses.
  + The districts with the highest number of apartments are Cầu Giấy, Hoàng Mai, Nam Từ Liêm, and Bắc Từ Liêm.
  + In contrast, outer districts, such as Đông Anh and Long Biên, primarily feature land for sale, with Đông Anh having the highest number of listings. In some other suburban districts, land sales account for the majority or even almost the entirety of real estate listings.

#### 2. Price and square of real estates
- The prices and squares of real estates in Hanoi are distributed across a very broad range, showing a high level of diversity and variability among the data points. This indicates that there is significant variation in both the cost and the area of properties available for sale across different neighborhoods and districts in the city.
  
![image](https://github.com/user-attachments/assets/f208e3a9-e7ba-422d-a94e-f36ff3a6fe70) ![image](https://github.com/user-attachments/assets/e07ba0c1-44c3-4f84-81ea-4e45b346b9c2)

- There is no clear correlation between the price and square of real estate properties across the entire scope of Hanoi. This suggests that real estate prices in Hanoi are influenced more significantly by other factors such as location, amenities, and property type rather than just the size of the property alone.
  
![image](https://github.com/user-attachments/assets/96f4f2bd-627e-436e-a12c-04a717747f9a)

- The type of real estate plays a significant role in determining property value. Apartments tend to have the lowest price distribution, while properties with street-facing houses (Nhà mặt tiền) exhibit a broader and higher price range.
  + Location is another crucial factor, as real estate prices vary considerably across different districts. In the central districts, for instance, properties in Hoàn Kiếm stand out with particularly higher prices compared to other districts, highlighting the influence of location on property values.
![image](https://github.com/user-attachments/assets/c5835c6c-1f21-44e1-9e21-eb5911b78138) ![image](https://github.com/user-attachments/assets/7a77b749-fabb-4897-abdc-ea4612a5e2b7)

![image](https://github.com/user-attachments/assets/d7bd0db2-97a1-4110-9228-18de5d68243a) ![image](https://github.com/user-attachments/assets/f52612c9-5457-4085-856b-098360528f8a)



#### => Conlusion:
  + In terms of the total value of properties listed for sale, Cầu Giấy ranks first when it also has the highest number of real estate listings.
  + Disregarding the quantity factor and focusing on the price per square meter, properties in Hoàn Kiếm have the highest prices. This district, located in the heart of the city, boasts some of the oldest streets, and most of the real estate comprises street-facing properties. The prices here can be exceptionally high, reaching over 500,000,000 VND per square meter, demonstrating the premium placed on prime, central locations.

#### 3. Time
- The trend indicates that real estate prices in Hanoi are gradually increasing over time, with a particularly significant rise in Hoàn Kiếm District. This suggests that properties in central, historically significant areas like Hoàn Kiếm are becoming even more valuable, reflecting the growing demand and limited availability in these prime locations.
  
![image](https://github.com/user-attachments/assets/8ae00771-d155-434d-81d8-8c8df9e72942) ![image](https://github.com/user-attachments/assets/2767dc94-0b5e-432d-9565-6967f70c90ae)



