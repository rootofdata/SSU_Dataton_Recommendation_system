# SSU_Recommendation_system
**Developing a recommendation system and implementing a service using library data provided by SSU Data Competition**
- Activating library homepage use through recommendation system development
  
## Idea details

### Background:
The utilization of library apps and websites has seen a decline due to the COVID-19 pandemic. Consequently, many students are unaware of the advantages offered by these platforms, resulting in limited access to various services. While features like e-learning and paper searches are relatively well-utilized, interest in book borrowing remains notably low.

### Key Strength of Central Libraries: Information Gathering
According to research on "The Impact of School Libraries on Students' Academic Achievement," methods that involve collecting and utilizing information and resources can positively influence students' academic performance. To address this, we aim to introduce a book recommendation service on the central library's website to measure the concrete results of specific recommendation policies through consumer needs identification and satisfaction surveys.

### Objectives:
**Enhancing the Book Abilities of University Students:**
- Leveraging accumulated book borrowing data to activate library services.
- Developing a recommendation system to provide convenient and beneficial information about tailored books.
- Stimulating student interest through supplementary library services.  

**Activation of University's Smart Campus:**
- Encouraging the use of the library app and website through related book recommendations.
- Facilitating early stocking of popular library books.
- Providing valuable library services to activate the smart campus.

### Detailed Plan:
We will employ "Central Library Single Book Borrowing" and "Central Library Single Book Reservation" data, alongside the Interpark Open API, to calculate scores. We will develop a recommendation model to determine suitable books for users based on user or book similarities, utilizing various recommendation policies.

We will conduct surveys to determine the most appealing approach for University students and incorporate this scenario into the app. Subsequently, we will measure user satisfaction as a quantitative metric to evaluate the impact of introducing recommendation policies.

The recommendation model will be developed using the Python framework Surprise. Upon completion, it will be integrated into the app and website, offering users personalized book recommendations.

This project aims to stimulate students' interest in reading, boost library usage, and enhance the overall academic experience, ultimately contributing to the activation of University's smart campus.

## Model Process

**Problem Definition (Storytelling)**:**
- **A(Data Planning)**: Survey Data - Satisfaction survey of the existing library website (to determine the direction of recommendations).
Y(Used as Evaluation Metric): Average Satisfaction (used as a quantitative evaluation metric).
- **B(Problem Definition)**: QFD (Quality Function Deployment) → A tool for identifying equipment characteristics based on customer needs.

**Hypothesis and Data Collection:**
- **C(Setting Hypothesis)**: Calculate Rating Data (Self-calculated: number of loans + Interpark Rating API).
- **D(Data Preparation)**: Generate User, Item, Rating columns as final modeling data.

**Conclusion Drawing:**
- **E(Modeling)**: Generate the final scoring data (User-Item(Book)-Rating(Self-scoring)).
Compare model performance (KNN, SVD, NMF) using the Surprise library.
Fine-tuning: Hyperparameter tuning, k-fold validation, etc., for improved model performance.
Compare the performance of similarity functions (Cosine, msd, Pearson) as different similarity functions have different criteria.
e.g., Cosine: Similarity based on slopes, Pearson: Similarity based on the absolute difference of coordinates.
- **F(Conclusion Drawing)**: Compare model performance using metrics such as RMSE, MAE, and adopt the best-performing model.

**Effect Verification:**
- **G(Implementation)**: Develop app scenarios and recommendation use cases.
- **H(Effect Verification)**: Survey Data 2: Verify the effect of library website satisfaction survey.
Compare initial Y and calculate expected improvement in satisfaction.
Note: This process outlines how to approach the problem, collect and preprocess data, build models, and verify their effectiveness in improving library website usage and satisfaction.

### University Central Library Datathon Excellence Award
(Customized book recommendation service for students)
- SSU Datathon Excellence Award
- Published by: Soongsil University · August 2022
