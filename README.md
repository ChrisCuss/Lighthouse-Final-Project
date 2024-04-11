# Lighthouse-Final-Project
## Project Title:
Customer Segmentation for Siempre Tequila Sales Enhancement

## Goal:
The goal of this project is to boost Siempre Tequila's customer engagement and sales strategies by employing advanced machine learning to segment customers based on their purchasing behavior. By understanding distinct customer groups, we aim to enable more personalized sales approaches, enhancing customer satisfaction and loyalty, and ultimately driving sales growth.

## Project Description:
Facing challenges in engaging customers efficiently, this project seeks to leverage Siempre Tequila’s extensive dataset on customer transactions and sales. We will use unsupervised learning, specifically k-means clustering, to segment the customer base into unique groups characterized by their buying habits and preferences. This strategic segmentation will uncover various customer types, empowering the sales team to tailor their strategies and communications effectively for each group. The initiative is set to improve customer experiences, foster loyalty, and stimulate sales expansion by catering to the specific needs and preferences of each segment.

## Data Utilization:
To achieve our objectives, we will analyze Siempre Tequila’s rich customer and sales data, which includes:

- **Dist. STATE**: The state or district where the customer is located, indicating the customer's geographical area.
- **Account ID**: Unique identifier for each customer account, used for tracking individual customer data.
- **City**: The city of the customer's location, providing further geographical specificity.
- **OnOff Premises**: Indicates if purchases are made on-premise (e.g., bars, restaurants) or off-premise (e.g., retail stores).
- **Classes of Trade**: Type of customer business or venue, such as restaurant, bar, or retail store, for targeted strategies.
- **Siempre Plata**: Volume of Siempre Plata purchased, reflecting preference for this product variant.
- **Siempre Reposado**: Volume of Siempre Reposado purchased, indicating demand for this variant.
- **Siempre Anejo**: Purchased volume of Siempre Anejo, showing preference for the Anejo variant.
- **Siempre Supremo**: Volume of Siempre Supremo purchased, tracking demand for this higher-end variant.
- **Siempre Rebel Cask**: Purchased volume of Siempre Rebel Cask, indicating interest in this special edition variant.
- **Siempre Exclusivo Vivo**: Volume of Siempre Exclusivo Vivo purchased, highlighting interest in this exclusive variant.
- **Total Cases**: Total number of cases purchased across all variants, measuring overall volume of purchases.
- **Did Buys**: Binary indicator (1 for Yes, 0 for No) showing if the customer made any purchases in a specific period.
- **# Purchases**: Total number of purchase transactions by the customer, counting transactions rather than volume.
- **# Months Purchased**: Number of distinct months with at least one purchase, indicating purchase frequency.
- **Rate of Sale: Units / Month**: Average monthly purchase rate, offering insights into buying patterns over time.
- **Ave Unit Price**: Average price per unit paid by the customer, providing an understanding of price sensitivity or premium product preference.

Utilizing this comprehensive dataset, we aim to deeply understand and segment Siempre Tequila’s customer base, laying the groundwork for targeted sales strategies and marketing initiatives.

## Disclaimer

For this project, I made sure to protect the privacy of Siempre Tequila's customers and the company's intellectual property. I've either removed or made anonymous any personal information in the dataset we analyzed. The aim was to make sure we couldn't identify any customers directly and that any findings we shared didn't give away Siempre Tequila's confidential info. Keeping customer privacy and the company's intellectual property safe was a key priority throughout our analysis and in how we reported our findings.

## Project Steps:
- **Imported Libraries**: Loaded Python libraries for data analysis and machine learning.
- **EDA**: Conducted exploratory data analysis to understand data distributions.
- **Data Cleaning**: Handled missing values and data inconsistencies.
- **Outlier Detection**: Managed outliers to prevent skewing the analysis.
- **Feature Selection**: Chose relevant features for clustering.
- **Encoding & Scaling**: Prepared data through encoding and scaling.
- **K-Means Clustering**: Segmented the customer base into distinct groups.
- **Optimal Number of Clusters**: Determined the ideal number of clusters.
- **Cluster Analysis**: Developed profiles for each customer segment.
- **PCA**: Applied Principal Component Analysis for dimensionality reduction.
- **Cluster Profiles**: Created detailed profiles based on segment characteristics.

## Cluster Profiles and Strategic Insights:

### Cluster 1: Low Volume Clients
- **Purchasing Behavior:** These clients make selective purchases, typically aligned with specific events or seasons of the year. Possibly also only purchasing when special deals are offered.
- **Client Profile:** Primarily event organizers and small restaurant owners who seek distinctive offerings to enhance their events.
- **Strategy Insight:** Highlighting product exclusivity and offering event-centric promotions could effectively engage this segment.

### Cluster 2: Niche Hospitality Venues
- **Purchasing Behavior:** Demonstrates a preference for quality, with purchases made on a more regular basis than the first group, though still selective.
- **Client Profile:** Includes boutique bars and specialized venues that aim to provide unique experiences to their patrons.
- **Strategy Insight:** Providing exclusive products and marketing support can help these establishments elevate their customer experience.

### Cluster 3: Volume Purchasers
- **Purchasing Behavior:** Characterized by consistent, high-volume purchases for resale or supply to large-scale sales volumes.
- **Client Profile:** This group consists of wholesalers, retail outlets, and major event organizers seeking reliable bulk purchasing options.
- **Strategy Insight:** Offering volume discounts, ensuring consistent supply, and providing marketing materials can strengthen partnerships.

### Cluster 4: Retail and Hospitality Chains
- **Purchasing Behavior:** Exhibits very high purchase volumes, indicating a steady demand for business operations or corporate events.
- **Client Profile:** Comprises large chain corporations, hospitality chains, and institutional clients with varied needs.
- **Strategy Insight:** Tailored account management and bespoke product offerings can meet their diverse requirements and foster long-term relationships.

### Cluster 5: Luxury and Premium Segment
- **Purchasing Behavior:** Prefers premium products, focusing on quality and exclusivity to enhance their high-end service offerings.
- **Client Profile:** Luxury hotels, upscale restaurants, and exclusive clubs seeking to offer premium experiences.
- **Strategy Insight:** Developing exclusive product lines or experiences tailored for the luxury market can offer competitive advantages.

## Technical Challenges and Solutions
During the project, we encountered several technical challenges that required creative and effective solutions:

- **Data Preprocessing Complexity**: Faced with a dataset full of missing values and outliers, I perfomed EDA and Data Cleaning techniques, ensuring a clean dataset for analysis.
- **Determining the Optimal Number of Clusters**: The Elbow Method was instrumental in identifying the most appropriate number of clusters, balancing between too many segments and too few.
- **High Dimensionality of Data**: Applied PCA to reduce the dataset to a more manageable size without significant loss of information, facilitating better visualization and interpretation of clusters.
- **Integrating Domain Knowledge**: Worked closely with my colleague, Rick from Siempre Tequila to ensure that the segmentation was aligned with business goals and industry insights, making the results actionable.

## Conclusion:
The segmentation enhances our understanding of the customer base, enabling targeted engagement to improve satisfaction, loyalty, and sales.

## Future Directions:
- Monitor and adapt segmentation strategies as needed.
- Explore additional analytics techniques for deeper insights.
- Implement insights across marketing and sales strategies.

