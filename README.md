# Big_data

# Mall Customers Segmentation using Self-Organizing Map (SOM)

## Project Overview
This project uses the **Mall Customers Dataset** to perform **customer segmentation** using a **Self-Organizing Map (SOM)**. The goal is to identify different customer segments based on their age, annual income, and spending score, which can help businesses better understand their customers and develop targeted marketing strategies.

### Key Objectives:
- Identify and segment customers based on `Age`, `Annual Income (k$)`, and `Spending Score (1-100)`.
- Utilize a Self-Organizing Map (SOM) to map the customer data onto a grid and form clusters.
- Visualize the SOM results to interpret different customer segments.

## Dataset Description
The dataset contains 200 entries with the following attributes:

| Column Name             | Description                                       |
| ----------------------- | ------------------------------------------------- |
| `CustomerID`             | Unique identifier for each customer               |
| `Gender`                 | Gender of the customer                           |
| `Age`                    | Age of the customer                              |
| `Annual Income (k$)`     | Annual income of the customer in thousands        |
| `Spending Score (1-100)` | A score assigned based on customer behavior       |

**Data Source:** [Kaggle - Mall Customers Dataset](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python)

### Features Used for Segmentation:
1. **Age** - The age of the customer.
2. **Annual Income** - The yearly income of the customer in thousands of dollars.
3. **Spending Score** - A score between 1 and 100 that reflects customer spending behavior.

## SOM Implementation
The **Self-Organizing Map (SOM)** is a type of unsupervised learning used to cluster the customers. It maps multidimensional data onto a two-dimensional grid while preserving the topological properties of the data. 

- **Grid Size**: The SOM was set up on a **10x10 grid**, meaning the map consists of 100 neurons.
- **Iterations**: The SOM was trained with 1000 iterations.
- **Input Features**: We used three features: `Age`, `Annual Income`, and `Spending Score`.

### Purpose of SOM:
- **Customer Segmentation**: Identify clusters of customers based on their similarities in the selected features.
- **Data Visualization**: Use SOM to visualize the distribution and relationships of customer groups on the grid.

## Visualizations
Several visualizations were created to interpret the SOM clusters and gain insights into customer behavior:

### 1. **SOM Clusters**
Displays how the customers are distributed across the SOM grid, showing potential clusters and customer groups.

### 2. **U-Matrix (Distance Matrix)**
The U-Matrix visualizes the distance between neurons (customer clusters) on the SOM grid. Larger distances indicate distinct clusters, while smaller distances suggest similar groups.

### 3. **Neuron Activation Frequency**
Shows how frequently each neuron in the SOM grid is activated (i.e., how many customers fall into each cluster). Neurons with higher activations represent denser customer clusters.

## Conclusion
The project successfully demonstrates customer segmentation using a Self-Organizing Map. The visualizations highlight distinct customer groups based on their age, income, and spending habits, which can be valuable for targeted marketing and business strategies.

