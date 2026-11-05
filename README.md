ProfitPulse analyses the direct marketing campaigns of a Portuguese bank to understand which customers subscribe to term deposits, and predicts future subscribers using distributed machine learning on Apache Spark.

The project processes 45,211 customer records through 15 structured objectives, from data quality checks and customer segmentation (age, job, education, loans, contact method, campaign month) to a leak-free Spark MLlib pipeline. Key findings include a 64.73% subscription rate among customers whose previous campaign succeeded, and a 33.63% rate among customers aged 60 and above, against an overall rate of just 11.70%.

Two classifiers were compared on the same test set. Logistic Regression achieved the best ROC-AUC (0.7725), while the Decision Tree found more than twice as many actual subscribers (20.84% recall vs 9.67%). Because always predicting “no” already gives 88.91% accuracy, models were judged on precision, recall, F1 and PR-AUC, not accuracy alone.

Tech stack: Apache Spark 4.2.0 · PySpark · Spark SQL · Spark MLlib · Python 3.12
