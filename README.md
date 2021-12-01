# Post Test Score Prediction

## Problem Framing
### a. Business Objective
From this project, we hope to find the factors that affect students' performance the most.

### b. Output
The goal is to predict students' performance (judged by their post-test score) based on the learning environment that they are in. We also want to optimize the learning environments so it can increase students' ability to study.

### c. What Maching Learning Task
We are using supervised learning, specifically regression. We are going to predict the post-test score as the label, which we already have from the available dataset, so we are using supervised learning. As the label is continuous numerical feature, we are going to be using regression. We are choosing from multiple models and finding out the best performing model.

### d. Performance Measure
We can use R-squared to measure our model's goodness of fit and RMSE to measure how much error the model predicts.

### e. Risks
Risks when our model produces wrong prediction can be development in the wrong categories. For example if our model predicts that school setting has a high impact on students' performance, it could lead to future schools being built in only certain areas when in fact it does not have any impact on the performance. It could in turn affect future students because they may have to commute longer to their schools.

## Result, Conclusion, Recommendation
<img src=Images/Post Test Coef.png>
<img src=Images/Post Test Formula.PNG>

From the linear equation with R<sup>2</sup> 94% and RMSE 3.2, we are confident in saying that:

* The base post-test score is 22.51
* It increases by 0.69 if the school setting is in the Suburban area and by 0.119 if in the Urban area
* The score decreased by 0.05 if the school is a public school
* Standard teaching method decreases the score by 6.06
* If the student is Male, the score decreases by 0.08
* If the student qualifies for reduced/free lunch, it further decreases by 0.955
* A one-student increase in the n_student in the classroom also decreases the score by 0.07
* Higher pretest score also means higher posttest score, in that for every 1 score increase in pretest, the student will have 0.91 increase in posttest.
From the equation, we can see that teaching_method affects the post-test scores the most, the the next most influential aspect is is the students qualify for free lunch. This aspect represents the students' economic background, meaning that students from lower economic ability usually have lower test scores.

From this result, we can implement certain things to improve and balance students' learning ability (as shown by the post-test score). For example, implementing more experimental teaching methods in all schools, finding out the reasons why students from lower economic background have more trouble studying and improving that aspect, building more schools in the suburban area, and decreasing the number of students in a class.

From the equation, we can see that teaching_method affects the post-test scores the most, the the next most influential aspect is is the students qualify for free lunch. This aspect represents the students' economic background, meaning that students from lower economic ability usually have lower test scores.

From this result, we can implement certain things to improve and balance students' learning ability (as shown by the post-test score). For example, implementing more experimental teaching methods in all schools, finding out the reasons why students from lower economic background have more trouble studying and improving that aspect, building more schools in the suburban area, and decreasing the number of students in a class.
