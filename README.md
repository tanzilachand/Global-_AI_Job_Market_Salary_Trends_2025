# Project XYZ

**Global AI Job Market & Salary Trends 2025** is a comprehensive data analysis tool designed to streamline data exploration, analysis, and visualisation. The tool supports multiple data formats and provides an intuitive interface for both novice and expert data scientists.

## Table of Contents
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
|salary_usd|	Annual salary in USD|	Integer
|salary_currency|	Original salary currency|	String
|salary_local|	Salary in local currency|	Float
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

## Business Requirements
* Describe your business requirements


## Hypothesis and how to validate?
* List here your project hypothesis(es) and how you envision validating it (them) 

## Project Plan
* Outline the high-level steps taken for the analysis.
* How was the data managed throughout the collection, processing, analysis and interpretation steps?
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
