# Netflix Dataset Analysis using Amazon QuickSight

Amazon QuickSight helps you analyze data and create visualizations easily. In this project, we will analyze a large dataset of Netflix shows and movies to create a dashboard that extracts meaningful insights. 🥝

Even if you're not familiar with data analysis, Amazon QuickSight is designed to be beginner-friendly. This project will guide you through the steps to create insightful dashboards in no time!

## Project Overview

In this project, you will:

- 🪣 Upload a dataset into an S3 bucket.
- 🆕 Create an account on Amazon QuickSight.
- 🔗 Connect your dataset (stored in the S3 bucket) to Amazon QuickSight.
- 📊 Create a variety of graphs, charts, and analyses using QuickSight.

## Step-by-Step Instructions

### Step 1: Download the Dataset

- Download the **netflix_titles.csv** file. This contains all the data for analysis. [Download Link](https://storage.googleapis.com/nextwork_course_resources/courses/aws/AWS%20Project%20People%20projects/Project%3A%20Visualise%20Data%20using%20Amazon%20QuickSight/netflix_titles.csv) (Right-click, and select "Save Link As").
- Download the **manifest.json** file. [Download Link](https://storage.googleapis.com/nextwork_course_resources/courses/aws/AWS%20Project%20People%20projects/Project%3A%20Visualise%20Data%20using%20Amazon%20QuickSight/manifest.json) (Right-click, and select "Save Link As"). We will explain why this file is important in the later steps!

### Step 2: Store the Dataset in Amazon S3

1. Log in to your AWS Account and open the **S3 console**.
2. Create a new S3 bucket:
   - Name the bucket as `nextwork-quicksight-yourname` (replace "yourname" with your actual name).
   - Choose a region closest to you.
   - Keep the other settings as default and create the bucket.
3. Upload the **netflix_titles.csv** and **manifest.json** files into the bucket.
4. Copy the S3 URL of your **netflix_titles.csv** file.
5. Open the **manifest.json** file using a text editor (TextEdit on Mac, Notepad on Windows).
   - Replace the URL in the **manifest.json** with the S3 URL of your dataset.
   - Re-upload the modified **manifest.json** back into your S3 bucket, which will replace the existing one.

💡 **Why are we using Amazon S3?**
We are storing the dataset in an S3 bucket, and later QuickSight will connect to it to fetch the data and create visualizations.

### Step 3: Create Your Amazon QuickSight Account

1. Search for **Amazon QuickSight** in the AWS console.
2. Sign up for QuickSight:
   - Choose the **Enterprise Edition** for the free trial.
   - Uncheck the upgrade offer.
3. Enter your QuickSight account details (make sure to use the same email as your AWS account).
4. Connect QuickSight to your S3 bucket:
   - Select **Amazon S3**.
   - Tick the box for the S3 bucket you created.
   - Click **Create**.
5. Wait a minute for your account to be ready, then click **Go to Amazon QuickSight**.

### Step 4: Connect Your S3 Bucket to Amazon QuickSight

1. From the left-hand navigation bar in QuickSight, select **Datasets**, then click **New dataset**.
2. Select **S3** as your data source.
3. For the first field (source name), enter `kaggle-netflix-data`.
4. In the **manifest.json URI** field:
   - Go back to your AWS S3 bucket.
   - Copy the S3 URI of the **manifest.json** file.
   - Paste the S3 URI into the **manifest.json URI** field.
5. Click **Connect**. Success! 🎉

💡 **What does the manifest.json file do?**
The `manifest.json` file acts like a map that tells Amazon QuickSight where the data is stored and how to read it. It helps QuickSight interpret the dataset so it can create accurate visualizations.

### Step 5: Visualize Netflix Data

1. Click **Visualize** to start creating charts and graphs from the dataset.
2. Explore the trends in Netflix movies, TV shows, genres, release years, and more.
3. Add the following visualizations to your dashboard:
   - Bar charts for the number of movies vs. TV shows.
   - Pie charts for the distribution of genres.
   - Time series to show the release trends over the years.
4. Customize your dashboard to extract the most valuable insights.

## Conclusion

After following these steps, you'll have a fully functional dashboard that provides insights into Netflix's library of shows and movies using Amazon QuickSight. 🎬

Feel free to explore more features of QuickSight and add additional analyses or visualizations to your project.

## Screenshots

Add screenshots of your final dashboard here to show the trends of Netflix movies, TV shows, genres, and more.

---

Happy Visualizing! 🚀
