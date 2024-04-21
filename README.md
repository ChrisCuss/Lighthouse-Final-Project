# Lighthouse-Final-Project
## Project Title:
Customer Segmentation for Siempre Tequila Sales Enhancement

## Disclaimer

For this project, I made sure to protect the privacy of Siempre Tequila's customers and the company's intellectual property. I've either removed or made anonymous any personal information in the dataset we analyzed. Additionally, some of the data has been either changed or randomized to ensure further protection of Siempre's IP. The aim was to make sure we couldn't identify any customers directly and that any findings we shared didn't give away Siempre Tequila's confidential information. Maintaining the privacy of customer data and safeguarding the company's intellectual property were key priorities throughout our analysis and in how we reported our findings.

## Goal:
The goal of this project is to boost Siempre Tequila's customer engagement and sales strategies by employing advanced machine learning to segment customers based on their purchasing behavior. By understanding distinct customer groups, we aim to enable more personalized sales approaches, enhancing customer satisfaction and loyalty, and ultimately driving sales growth.

## Project Description:
Facing challenges in engaging customers efficiently, this project seeks to leverage Siempre Tequila’s extensive dataset on customer transactions and sales. We will use unsupervised learning, specifically k-means clustering, to segment the customer base into unique groups characterized by their buying habits and preferences. This strategic segmentation will uncover various customer types, empowering the sales team to tailor their strategies and communications effectively for each group. The initiative is set to improve customer experiences, foster loyalty, and stimulate sales expansion by catering to the specific needs and preferences of each segment.

## Technologies Used

This project was built using the following technologies:

- **Python**: Main programming language used for backend calculations and data processing.
- **Pandas**: Utilized for data manipulation and analysis.
- **NumPy**: Employed for numerical data operations.
- **Scikit-learn**: Used for machine learning models and data preprocessing.
- **Matplotlib** and **Seaborn**: For generating visualizations in the Jupyter Notebook.
- **Jupyter Notebook**: Interactive computing and development environment.
- **Git**: Version control system.
- **GitHub**: For repository hosting.
- **Visual Studio Code**: Preferred code editor.
- **VIP/iDIG**: Main reporting tool for the Wine & Spirits industry in the USA.
- **Tableau**: Tool for data visualization.
- **Microsoft PowerPoint**: Used for creating the presentation slides.

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

## Imported Libraries

![Alt Text](https://github.com/ChrisCuss/Lighthouse-Final-Project/blob/main/Images/Imported%20Libraries.png?raw=true)

## Feature Selection

Considering the project's goal, the below features are most relevant for customer segmentation based on purchasing behavior:

- **OnOff Premises**
- **Classes of Trade**
- **Siempre product columns (e.g., Siempre Plata, Siempre Reposado, etc.) for understanding product preferences**
- **Total Cases**
- **Purchases**
- **Months Purchased**
- **Rate of Sale: Units / Month**
- **Ave Unit Price**

## Encoding & Scaling

For Encoding and Scaling, I used sklearn's StandardScaler() for the numerical features and OneHotEncoder() for the categorical features.

![Alt Text](https://github.com/ChrisCuss/Lighthouse-Final-Project/blob/main/Images/Encoding%20&%20Scaling.png?raw=true)

## K-Means Clustering

### Determining the Optimal Number of Clusters

By using the ''Elbow Method'', I was able to determine that the optimal amount of clusters would be 5.

![Alt Text](https://github.com/ChrisCuss/Lighthouse-Final-Project/blob/main/Images/Elbow%20Method.png?raw=true)

### Running KMeans Clustering

![Alt Text](https://github.com/ChrisCuss/Lighthouse-Final-Project/blob/main/Images/Running%20KMeans%20Clustering.png?raw=true)

### Analyzing the Clusters

Next, I took a look at the mean of each cluster and started creating customer profiles based on the results.

![Alt Text](https://github.com/ChrisCuss/Lighthouse-Final-Project/blob/main/Images/Analyzing%20the%20Clusters.png?raw=true)

# Key Findings and Data Vizualisation

## Cluster Profiles and Strategic Insights:

### Cluster 0: Low Volume Clients
- **Purchasing Behavior:** These clients typically buy less and often only during specific times like special events or when there are discounts. They're not frequent buyers and usually make smaller purchases compared to others.
- **Client Profile:** Mostly made up of small event organizers, and owners of little shops and restaurants who are looking for unique Tequila options.
- **Strategy Insight:** To really get this group's attention, we could roll out special offers and engaging promotions. Focusing on increasing our visibility during their slow times or off-peak hours might also help boost their purchases.

### Cluster 1: Niche Hospitality Venues
- **Purchasing Behavior:** This group tends to prefer quality over quantity, buying more regularly than the first group but still choosing selectively. Their purchases are generally below average, which might indicate a sensitivity to prices or a limited selection.
- **Client Profile:** Comprised of boutique bars, especially those with a focus on Tequila or Mexican themes, and other specialized venues.
- **Strategy Insight:** To enhance their experience and satisfaction, we could offer exclusive products and provide dedicated marketing support to these venues.

### Cluster 2: Volume Purchasers
- **Purchasing Behavior:** This cluster shows consistent, high-volume purchasing habits, ideal for resale or supplying large events. They frequently buy a wide range of products, including high amounts of premium lines like Siempre Anejo and Siempre Exclusivo Vivo.
- **Client Profile:** Made up of wholesalers, large retail outlets, and organizers of major events who need reliable bulk purchasing options.
- **Strategy Insight:** Strengthening relationships with these customers can be achieved by offering volume discounts, ensuring a consistent supply, and providing tailored marketing support. Keeping supply reliable, prioritizing these customers for new launches, and recognizing their needs with discounts are key to keeping them engaged.

### Cluster 3: Retail and Hospitality Chains
- **Purchasing Behavior:** Characterized by extremely high purchase volumes, these clients consistently demand products for business operations and corporate events.
- **Client Profile:** Includes large chain corporations, hospitality chains, and institutional clients, each with diverse and specific needs.
- **Strategy Insight:** Effective strategies include tailored account management and bespoke product offerings designed to meet their varied requirements. Strengthen relationships through customized partnership plans, reliable supply chains, and exclusive business buyer programs. Additionally, consider developing unique marketing collaborations, particularly for restaurants and tasting rooms, to enhance their customer experiences.

### Cluster 4: Luxury and Premium Segment
- **Purchasing Behavior:** This cluster shows a strong preference for premium products, with a significant focus on quality and exclusivity. Notably high purchases of Siempre Supremo and Siempre Rebel Cask highlight their orientation towards luxury and premium offerings.
- **Client Profile:** Composed of luxury hotels, upscale restaurants, and exclusive clubs, all dedicated to providing top-tier experiences.
- **Strategy Insight:** To stay competitive and appealing to this segment, developing exclusive product lines or bespoke experiences tailored to the luxury market is essential. These initiatives should emphasize uniqueness and high quality, aligning with the expectations of luxury consumers.

## Data Vizualisation

![Alt Text](https://github.com/ChrisCuss/Lighthouse-Final-Project/blob/main/Images/%25%20of%20Total%20Sales%20by%20Cluster.png?raw=true)

![Alt Text](https://github.com/ChrisCuss/Lighthouse-Final-Project/blob/main/Images/Total%20Case%20Sales%20by%20Cluster.png?raw=true)

![Alt Text](https://github.com/ChrisCuss/Lighthouse-Final-Project/blob/main/Images/AVG%20Rate%20of%20Sale%20by%20Cluster_2.png?raw=true)

![Alt Text](https://github.com/ChrisCuss/Lighthouse-Final-Project/blob/main/Images/%25%20Of%20Customers%20by%20Cluster.png?raw=true)

![Alt Text](https://github.com/ChrisCuss/Lighthouse-Final-Project/blob/main/Images/AVG%20%23%20Months%20Purchased%20by%20Cluster_2.png?raw=true)

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

