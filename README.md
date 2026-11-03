# Week 3 — Unsupervised Learning and Customer Clustering

## Objective
Apply unsupervised learning to discover customer segments using profile and campaign-history attributes, without using the known subscription outcome.

## Files
- `YuvaIntern3_week3.ipynb` — executed clustering notebook.
- `Week3_Unsupervised_Customer_Clustering_Report.docx` — detailed report.
- `bank_customer_clusters.csv` — passenger/customer-level cluster assignments.
- `bank_cluster_profiles.csv` — cluster summary statistics.

## Work Completed
- Mixed numeric/categorical feature preprocessing.
- Robust scaling and one-hot encoding.
- K-Means cluster-count comparison using inertia and silhouette.
- Five-cluster K-Means solution.
- Internal cluster evaluation.
- Cluster visualization using PCA.
- Cluster profiling and post-hoc outcome comparison.

## Verified Results
- Selected k: 5.
- Sampled silhouette score: 0.8880.
- Davies–Bouldin: 0.3404.
- Calinski–Harabasz: 24,776.67.
- Cluster sizes: 39,362; 207; 1,343; 2,182; 2,117.

## Important Interpretation
The largest cluster contains 39,362 customers (approximately 87.06%). This is a highly imbalanced segmentation and is discussed as a limitation. A high internal score alone does not prove practical segmentation value.

The target `y` and post-call variable `duration` are excluded from clustering inputs. Subscription rates are examined only after clusters are formed.

## Re-running
Open the notebook in Google Colab and select **Runtime → Run all**. The notebook exports cluster assignment and profile CSV files.
