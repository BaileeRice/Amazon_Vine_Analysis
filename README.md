# Amazon_Vine_Analysis

![image](https://user-images.githubusercontent.com/105184244/195554372-80ed7448-7c33-47d8-9664-4435de0a418e.png)

OVERVIEW:

Analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products.

I picked the 'Video Games' dataset and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Afterwards I used PySpark, Pandas, and SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset.

>Dataset Directory    https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt

---

-How many Vine reviews and non-Vine reviews were there?

![image](https://user-images.githubusercontent.com/105184244/195548403-1e2dd005-0fe8-48d7-80d1-66b7bf4a89ab.png) 

![image](https://user-images.githubusercontent.com/105184244/195548484-34a74a93-14b0-4d98-ad06-a500ea6ed354.png)


-How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

![image](https://user-images.githubusercontent.com/105184244/195548571-c4604607-a0c6-40e5-896f-e833841ee248.png)  ![image](https://user-images.githubusercontent.com/105184244/195548658-b52dd8d7-53da-4c29-87bd-e8d2b46abe98.png)


-What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

![image](https://user-images.githubusercontent.com/105184244/195548725-63949452-6cab-4d26-ab7b-6e4c20018cdd.png) ![image](https://user-images.githubusercontent.com/105184244/195548780-6a73dd0c-a0a7-4706-9cef-355f25261bb5.png)

---

SUMMARY:

The stats show that 51 percent of the paid reviews are giving 5* ratings, whereas the unpaid is only 39 percent, showcasing a relatively positive bias in reviews. 

Another way to pinpoint biases would be to pass in the other datasets into the template or joining some together with the same analysis. Looking into the occurance rate of the stars given and preforming summary statistics on them could provide better insight on the subject.

