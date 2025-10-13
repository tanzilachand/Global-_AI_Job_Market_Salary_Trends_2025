# Global AI Job Market & Salary Trends 2025

**Global AI Job Market & Salary Trends 2025** is a comprehensive data analysis tool designed to streamline data exploration, analysis, and visualisation. The tool supports multiple data formats and provides an intuitive interface for both novice and expert data scientists.

## Table of Contents
 <details>
  <summary>Click here to expand the contents</summary>

1. [Project Overview](#project-overview)
2. [Dataset Content](#dataset-content)
3. [Business Requirements](#business-requirements)
4. [Hypothesis and how to validate?](#hypothesis-and-how-to-validate)
5. [Project Plan](#project-plan)
6. [The rationale to map the business requirements to the Data Visualisations](#the-r       ationale-to-map-the-business-requirements-to-the-data-visualisations)
7. [Analysis techniques used](#analysis-techniques-used)
8. [Ethical considerations](#ethical-considerations)
9. [Dashboard Design](#dashboard-design)
10. [Unfixed Bugs](#unfixed-bugs)
11. [Development Roadmap](#development-roadmap)
12. [Deployment](#deployment)
    - [Heroku](#heroku)
13. [Main Data Analysis Libraries](#main-data-analysis-libraries)
14. [Credits](#credits)
15. [Acknowledgements (optional)](#acknowledgements-optional)   

</details>

## Useful Links

- [GitHub Repository](https://github.com/tanzilachand/Global-_AI_Job_Market_Salary_Trends_2025)
- [Project Board](https://github.com/users/tanzilachand/projects/4)

  
## Dataset Content
Global AI Job Market & Salary Trends 2025: Complete Analysis of 15,000+ Positions is a comprehensive dataset that contains detailed information about AI and machine learning job positions, salaries, and market trends across different countries, experience levels, and company sizes. Perfect for data science enthusiasts, career researchers, and market analysts for practice purposes.

### Dataset Description
#### What's Inside
It includes detailed salary information, job requirements, company insights, and geographic trends.
#### Key Features:
- 15,000+ job listings from 50+ countries
- Salary data in multiple currencies (normalized to USD)
- Experience level categorization (Entry, Mid, Senior, Executive)
- Company size impact analysis
- Remote work trends and patterns
- Skills demand analysis
- Geographic salary variations
- Time-series data showing market evolution

Columns Description
|Column|	Description|	Type|
|------|---------------|--------|
|job_id|	Unique identifier for each job posting|	String
|job_title|	Standardized job title|	String
|salary_usd|	Annual salary Converted into USD|	Integer
|salary_currency|	Original salary currency|	String
|experience_level|	EN (Entry), MI (Mid), SE (Senior), EX (Executive)|	String
|employment_type|	FT (Full-time), PT (Part-time), CT (Contract), FL (Freelance)|	String
|job_category|	ML Engineer, Data Scientist, AI Researcher, etc.|	String
|company_location|	Country where company is located|	String
|company_size|	S (Small <50), M (Medium 50-250), L (Large >250)|	String
|employee_residence|	Country where employee resides|	String
|remote_ratio|	0 (No remote), 50 (Hybrid), 100 (Fully remote)|	Integer
|required_skills|	Top 5 required skills (comma-separated)|	String
|education_required|	Minimum education requirement|	String
|years_experience|	Required years of experience|	Integer
|industry|	Industry sector of the company|	String
|posting_date|	Date when job was posted|	Date
|application_deadline|	Application deadline|	Date
|job_description_length|	Character count of job description|	Integer
|benefits_score|	Numerical score of benefits package (1-10)|	Float

## Business Requirements: AI Employment and Salary Insights

### Salary Determinants Analysis: 
Identify and quantify the key factors that most significantly influence AI-related job salaries.
- Analyze variables such as job title, education level, years of experience, company size, and industry sector.
- Use statistical methods or machine learning models to determine the relative impact of each factor.
- Present findings with clear, data-driven insights to guide compensation strategy and talent acquisition.

### Remote Work Trend Analysis:
 Investigate trends and patterns in remote AI-related job opportunities.
- Measure the growth of remote positions over time.
- Compare salary levels and job satisfaction between remote, hybrid, and on-site roles.
- Identify emerging remote-friendly regions or companies leading in remote hiring.
- Compare salary levels and job satisfaction between remote, hybrid, and on-site roles.
- Identify emerging remote-friendly regions or companies leading in remote hiring.

### Data Visualization and Reporting Standards:
Develop effective visualization techniques to communicate employment data insights.
- Use interactive dashboards and visual storytelling to present data.
- Implement charts (e.g., heatmaps, box plots, scatterplots) for salary distributions, trends, and geographic patterns.
- Ensure visual consistency, clarity, and accessibility across all reports and presentations.

### Predictive Modeling for Salary and Hiring Trends:
Build and evaluate predictive models to forecast AI job salaries and employment demand.
- Use regression or machine learning techniques.
- Report model performance using accuracy metrics (e.g., R², MAE, RMSE).
- Provide recommendations based on model predictions for workforce planning and policy decisions.

### Geographic and Market Insights:
Identify and interpret regional variations and unexpected patterns in AI employment data.
- Map salary, job density, and hiring trends across geographic areas.
- Highlight surprising or emerging hotspots for AI talent and industry growth.
- Use insights to inform regional investment, training, or recruitment strategies.

## Hypothesis and how to validate?

## Hypothesis 1. Identify Key Salary Determinants:

AI job salaries are primarily influenced by experience level, job title, company size, and education background.

**Preparations Needed:**

- Collect and clean AI job posting and employee salary data.
- Standardize variables (e.g., job titles, locations, experience ranges).
- Conduct feature engineering (e.g., encode categorical variables, handle missing data).

**Validation Approach:**

- Perform correlation and regression analysis to test statistical significance.
- Apply machine learning feature importance analysis (e.g., random forest or XGBoost).
- Compare results across multiple datasets for consistency.

**Acceptance Criteria:**

- At least 3 statistically significant factors identified (p < 0.05).
- Model explains ≥70% of salary variance (R² ≥ 0.7).
- Clear ranking of top influencing factors presented with visuals.

Requirement 2: Detect Patterns in Remote Work Trends

**Hypothesis 2:** Remote work opportunities in AI have increased significantly post-2020, with consistent or higher salaries compared to on-site roles.

Preparations Needed:

- Filter job listings by work mode (remote, hybrid, onsite).
- Segment data by year, job type, and region.
- Normalize salary comparisons by role and experience.

**Validation Approach:**

- Conduct time-series and comparative trend analysis.
- Use statistical tests (e.g., t-test) to compare salary distributions.
- Visualize trend lines for remote vs onsite job postings.

**Acceptance Criteria:**

- Statistically significant upward trend in remote job share identified.
- Salary parity or advantage for remote roles clearly demonstrated.
- Visual charts showing 3+ years of trend data included.

Requirement 3: Establish Best Visualization Techniques

**Hypothesis 3:** Interactive dashboards and comparative visualizations (box plots, heatmaps, geographic maps) are most effective for communicating employment insights.

Preparations Needed:

- Evaluate dataset structure and visualization requirements.
- Test different visualization tools (Tableau, Power BI, Plotly, etc.).
- Design prototype visuals with stakeholder feedback loops.

Validation Approach:

Conduct stakeholder usability testing.

Measure interpretation speed and clarity using feedback surveys.

Acceptance Criteria:

≥80% of stakeholders rate visualizations as “clear” or “highly effective.”

Visuals meet accessibility and readability standards.

All visuals dynamically reflect updated data sources.

Requirement 4: Evaluate Prediction Model Performance

**Hypothesis 4:**
A machine learning model (e.g., Random Forest, XGBoost, or Linear Regression) can accurately predict AI job salaries using structured features.

Preparations Needed:

Prepare training and test datasets.

Select and tune predictive algorithms.

Define evaluation metrics (MAE, RMSE, R²).

Validation Approach:

Cross-validation on multiple data samples.

Benchmark against baseline models (mean prediction, simple regression).

Compare model accuracy across iterations.

Acceptance Criteria:

Model achieves ≥80% prediction accuracy or R² ≥ 0.8.

Error metrics (MAE/RMSE) fall within acceptable tolerance (≤15% of salary mean).

Final model and feature weights documented for reproducibility.

Requirement 5: Discover Geographic Insights

Hypothesis:
Certain regions (including emerging markets) show unexpectedly high AI job concentrations or salary levels due to local policy, tech ecosystems, or remote flexibility.

Preparations Needed:

Enrich job data with geographic and economic indicators.

Standardize location data (country, state, city).

Integrate visualization layers (maps, choropleths).

Validation Approach:

Perform geospatial clustering and comparative regional analysis.

Identify statistical outliers and confirm through external data sources.

Acceptance Criteria:

At least 3 regions identified with surprising or notable trends.

Geographic data accurately mapped and validated.

Insights supported by quantitative and contextual explanations.

## Project Plan
* Outline the high-level steps taken for the analysis.
* How was the data managed throughout the collection, processing, analysis and interpretation steps?

Agile and Sprint methodologies were used to manage the project. The project was divided into several sprints, each focusing on specific tasks such as data collection, cleaning, analysis, and visualization. Regular meetings were held to review progress and adjust the plan as needed.

* Why did you choose the research methodologies you used?

## The rationale to map the business requirements to the Data Visualisations
* List your business requirements and a rationale to map them to the Data Visualisations

## Analysis techniques used
* List the data analysis methods used and explain limitations or alternative approaches.
* How did you structure the data analysis techniques. Justify your response.
* Did the data limit you, and did you use an alternative approach to meet these challenges?
* How did you use generative AI tools to help with ideation, design thinking and code optimisation?

## Ethical considerations
* Were there any data privacy, bias or fairness issues with the data?
* How did you overcome any legal or societal issues?

## Dashboard Design
* List all dashboard pages and their content, either blocks of information or widgets, like buttons, checkboxes, images, or any other item that your dashboard library supports.
* Later, during the project development, you may revisit your dashboard plan to update a given feature (for example, at the beginning of the project you were confident you would use a given plot to display an insight but subsequently you used another plot type).
* How were data insights communicated to technical and non-technical audiences?
* Explain how the dashboard was designed to communicate complex data insights to different audiences. 

## Unfixed Bugs
* Please mention unfixed bugs and why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a significant variable to consider, paucity of time and difficulty understanding implementation are not valid reasons to leave bugs unfixed.
* Did you recognise gaps in your knowledge, and how did you address them?
* If applicable, include evidence of feedback received (from peers or instructors) and how it improved your approach or understanding.

## Development Roadmap
* What challenges did you face, and what strategies were used to overcome these challenges?
* What new skills or tools do you plan to learn next based on your project experience? 

## Deployment
### Heroku

* The App live link is: https://YOUR_APP_NAME.herokuapp.com/ 
* Set the runtime.txt Python version to a [Heroku-20](https://devcenter.heroku.com/articles/python-support#supported-runtimes) stack currently supported version.
* The project was deployed to Heroku using the following steps.

1. Log in to Heroku and create an App
2. From the Deploy tab, select GitHub as the deployment method.
3. Select your repository name and click Search. Once it is found, click Connect.
4. Select the branch you want to deploy, then click Deploy Branch.
5. The deployment process should happen smoothly if all deployment files are fully functional. Click now the button Open App on the top of the page to access your App.
6. If the slug size is too large then add large files not required for the app to the .slugignore file.


## Main Data Analysis Libraries
* Here you should list the libraries you used in the project and provide an example(s) of how you used these libraries.


## Credits 

* In this section, you need to reference where you got your content, media and extra help from. It is common practice to use code from other repositories and tutorials, however, it is important to be very specific about these sources to avoid plagiarism. 
* You can break the credits section up into Content and Media, depending on what you have included in your project. 

### Content 

- The text for the Home page was taken from Wikipedia Article A
- Instructions on how to implement form validation on the Sign-Up page was taken from [Specific YouTube Tutorial](https://www.youtube.com/)
- The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)

### Media

- The photos used on the home and sign-up page are from This Open-Source site
- The images used for the gallery page were taken from this other open-source site



## Acknowledgements (optional)
* Thank the people who provided support through this project.
