<h1 align="center">MartDashX</h1>

# About MartDashX

MartDashX is a cutting-edge administrative dashboard designed to empower e-commerce businesses with insightful analytics, streamlined operations, and intelligent recommendations. Developed with a deep understanding of the unique challenges faced by e-commerce administrators, MartDashX is your trusted companion for harnessing the full potential of your online store.

## Tech Stack

**Web Application:** MERN Stack (MongoDB, Express.js, React, Node.js)

**Recommendation Model:** Python and Flask

In an era where data reigns supreme, MartDashX offers e-commerce businesses the tools they need to succeed. Join us on a journey towards data-driven excellence, improved decision-making, and sustained growth. Elevate your e-commerce store with MartDashX and take the next step towards a prosperous future.

## Key Features

- **Client Analysis:** MartDashX empowers you to understand your customer base at a granular level. By examining user behavior, purchase history, and preferences, you can create tailored marketing strategies and improve customer satisfaction.

- **Sales Analysis:** In the fast-paced world of e-commerce, keeping a close eye on sales performance is vital. MartDashX offers detailed sales reports, product performance metrics, and forecasting tools to help you optimize your inventory and boost revenue.

- **Admins Performance Analysis:** Your team is the backbone of your operation. MartDashX enables you to track the performance of your admin staff, identify areas for improvement, and ensure your e-commerce business runs smoothly.

- **Recommendation List:** Leveraging state-of-the-art SVD (Singular Value Decomposition) algorithms, MartDashX goes beyond basic product recommendations. It offers a sophisticated and personalized recommendation engine, which not only increases cross-selling and upselling opportunities but also enhances the user experience on your e-commerce platform.

<h2> Quick Walkthorugh</h2>

![5fd04a8a-6cbc-4507-b877-92a4434ac78e](https://github.com/Shounmay/MartDashX_Grid5.0/assets/85643531/a51eff8e-7f6d-4c4b-a83a-07cfc38406a3)



<h2>Approach to Recommendation Model</h2>
<h3>1. Data Exploration (EDA):</h3>
The dataset encompasses multiple facets of an e-commerce platform such as events (e.g., view, add to cart, purchase), item details, and category structures. Our exploratory analysis revealed:<br>
•<b>Events Distribution: </b>Visual representation of various user actions.<br>
•<b>Temporal Trends:</b> The flow and frequency of user events over time.<br>
•<b>Item Popularity:</b> Identifying the top viewed and sold items.<br>
•<b>Category Insights:</b> Recognizing the most viewed and transacted categories.<br>
<h3>2. Feature Engineering:</h3>
To enrich our predictive model, we transformed the raw data into more insightful features:<br>

•<b>User-based Features:</b> Captured user behavior metrics like average time spent on the platform and the average number of items viewed.<br>
•<b>Item-based Features:</b> Metrics indicating item popularity based on different user events.<br>
•<b>User-item Interaction Features:</b> Details on the frequency and duration between user-item interactions.<br>
<h3>3. Model Building & Evaluation:</h3>
Our modeling approach used the Singular Value Decomposition (SVD) technique.<br>
•<b>Choice of SVD:</b> SVD's ability to discern latent factors in user-item matrices made it an apt choice. Its performance in recommendation scenarios further justified our pick.<br>
•<b>Hyperparameter Precision:</b> The GridSearchCV ensured our SVD model was precisely tuned. Parameters like n_factors, n_epochs, lr_all, and reg_all were meticulously selected to get the best out of our model.<br>
•<b>Training Strategy:</b> With the best parameters identified, the model was trained to recognize patterns, behaviors, and nuances in user-item interactions.<br>
•<b>Evaluation Rigor:</b> The model was then evaluated using the Mean Absolute Error (MAE) metric. To get a more holistic view, we also formulated an Accuracy Score and a Normalized Prediction Score.<br>



To provide a user-friendly interface and a consolidated view of the prediction outcomes and e-commerce metrics, we've developed a state-of-the-art admin panel with the following features:<br>
•<b>Dashboard:</b> A centralized hub to get a snapshot of the overall e-commerce health.<br>
•<b>User Recommendations:</b> The heart of our solution, this page showcases the product recommendations for users, as derived from our SVD model. Here, you'll find pairs of user IDs alongside their recommended item IDs.<br>
•<b>Client Facing Products & Customers:</b> Overview of products available and details on the customer base.<br>
•<b>Transactions Overview:</b> A look into transactional patterns, offering insights into shopping behaviors.<br>
•<b>Sales Analytics:</b> Breakdown of sales, presented in daily and monthly overviews, to gauge business momentum.<br>
<h3> Data Context:</h3>
It's important to note that while our user recommendation page is powered by genuine insights derived from our model, data on other admin panel pages is real time ecommerce business data(refer Business Data in repository). For building our model we have used the data which is reffered from Kaggle and its factors and attributes which we have kept depends on the analysis of results which we got from the real time ecommerce business data.<br>
When equipped with a richer dataset, our model and platform are structured to be fully functional, scaling seamlessly to the data's granularity.
<h2>Model Data</h2>
https://drive.google.com/drive/folders/1mjblgY1C_C0fmyxYrfsoI21uMptBwRQu?usp=sharing
<h2>Deployed Link</h2>
https://martdashxtest.onrender.com/

