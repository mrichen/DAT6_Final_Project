#Predicting Turnover in an Organization

##I intend to create a model which can be used to predict which employees will leave an organization in a given time period.

Turnover is costly to any organization, unexpected turnover especially so. By examining trends in demographic, compensation, performance evaluation data, management, etc. I believe I can predict the likelihood that any particular employee will resign in a given year (or other period), which would allow management to intervene or begin succession planning.

##Data Sources
The data used will include:
--Basic demographic information (age, gender, marital status, number of dependents, location, level of education, etc.)
--Position information (Years of Education, Years of Experience typical for position, Job Title Modifiers (e.g. Senior, Principal, etc.) Management Level)
--Compensation information (Total compensation relative to industry/area, Raise frequency, etc.)
--Performance Evaluation information (Scoring on most recent performance reviews, Length of time since last promotion)
--Management information (Manager's most recent performance reviews, Turnover within the same or similar supervisory organizations, etc.)

I will be extracting the data from Workday (a cloud-based HRIS and Financials system) for a fictional company created for sales and training purposes, creating custom reports with the Workday report builder and publishing them as REST resources. The only external datasource I anticipate needing will be for industry salary data, which I'm investigating. Ideally this will come from a source like Salary.com, but BLS data is available if budget becomes a concern.

##Methods
I'm anticipating that this will primarily involve a large logistic regression after some initial PCA-type analysis to remove or collapse less significant attributes or features. My end product will be a per-worker score indicating a 'risk level', along with visualizations that may highlight trends or commonalities. 
