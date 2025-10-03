# 🛍️ Customer Segmentation Analysis with K-Means

A data-driven approach to segmenting mall customers for strategic marketing insights.

---

### **Project Summary**
This repository presents an unsupervised machine learning analysis to group mall customers into distinct clusters based on their purchasing behavior. By applying the K-Means algorithm to the customers' annual income and spending scores, we can identify key personas that the marketing team can target with tailored campaigns.

### **Methodology**

The project is structured as follows:

1.  **Data Loading**: We start with the `Mall_Customers.csv` dataset.
2.  **Optimal Cluster Selection**: The ideal number of clusters is determined using the **Elbow Method**, a heuristic that helps find the point of diminishing returns in model performance.
3.  **K-Means Modeling**: A `KMeans` model is initialized and fitted to the data.
4.  **Cluster Labeling**: Each customer in the dataset is assigned to one of the identified clusters.
5.  **Evaluation**: The **Silhouette Score** is calculated to provide a quantitative measure of cluster cohesion and separation.
6.  **Visualization**: The final segments are plotted for clear, actionable insights.

### **Key Findings**
The analysis revealed **5 well-separated customer segments**, each with unique characteristics.

| Cluster ID | Customer Profile         | Income Level | Spending Level |
| :--------: | ------------------------ | :----------: | :------------: |
|     0      | **Target/Priority** |     High     |      High      |
|     1      | **Standard** |   Average    |    Average     |
|     2      | **Careful/Thrifty** |     High     |      Low       |
|     3      | **Careless/Aspirant** |     Low      |      High      |
|     4      | **Sensible/Risk-Averse** |     Low      |      Low       |

**Silhouette Score:** A score of **~0.55** was achieved, indicating a reasonable and well-defined clustering structure.

![Customer Personas](https://placehold.co/700x500/2c5282/ffffff?text=Identified+Customer+Personas)

### **Running the Project**

**Prerequisites:**
- Python 3.x
- Jupyter Notebook

**Setup:**
```sh
# Clone the repository to your local machine
git clone [https://github.com/your-username/customer-segmentation.git](https://github.com/your-username/customer-segmentation.git)
cd customer-segmentation

# Install dependencies
pip install pandas scikit-learn matplotlib seaborn
