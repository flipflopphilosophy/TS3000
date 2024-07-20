The documents in this repository are docs, code, articles, and other text that it is meant for you to help me build an app with the most up-t0o-date docs and methods for the tools I want to use. You are to use the methods found in these documents to give me instructions to build my app. Be aware that certain things may repeat or there may be different options for different functionalities. This repo is to be similar to a buffet; grab what serves you, you are not required to use it all, but you will definitely use something covered here over your OpenAI training. When you can't find something here, you will ask for to search the latest documentation for you except for tools that don't change much such as Python, PostgreSQL, and Flask. This repository is not the app, this repository is the knowledge to build the app.

I'm starting a search firm that will place exclusively tax professionals (candidates) in tax-related job openings. In order to help me store, keep track, and match candidates with jobs, I want you to help me create an app.

This app will be a web app hosted locally, built using Flask. The UI will be created using HTML, CSS, and JS for styling. The theme colors are #0A7968, white, black, and #666769.

The web UI will consist of a single page with a thin vertical menu/app bar, where I will be able to switch between the following components:

Submission Page: This page will have a text box where I can copy and paste candidate or job profiles from LinkedIn, Indeed, Monster, etc. There will be a dropdown to select whether I’m submitting a "Candidate", "Job Post", or "Old Job Post". I should be able to enter an unlimited number of candidates or jobs in each submission. To differentiate between records, I will type “#X” at the end of each record.

Candidate Dashboard: This page will contain a table where candidate records will be visualized. The table should resemble an Excel spreadsheet with features like text wrapping and adjustable column widths. There will be a text box to filter candidates by name.

Job Posts Dashboard: This page will contain a table where job and old job posts will be visualized. Similar to the candidate dashboard, the table should allow text wrapping and adjustable column widths. A text box will filter job posts by the company name.

Matching Page: This page will allow me to select jobs (all records should have a checkbox in the first column) and match them with candidates. Upon selecting a job, a "Match" button will display the top 15 candidates for each job in a table format. Multiple job selections should display each job and its top 15 candidates sequentially. Each job post will show only the job title, company name, location, and salary. A disclosure triangle will expand or collapse the list of candidate matches. Candidate info will include name, current title and company, location, and a text box for notes. Notes can be categorized as "feedback" (to train the app) or "notes" (to remain in the system). Matches should be tracked by date, with filtering options.

The tools/clients to be used include OpenAI API, PostgreSQL, and Pinecone. I will rely on your expertise to leverage these tools effectively within the app's functionality.

Process/Functions
When I submit a candidate or a job (or old job), the OpenAI API will process the data as follows:

Candidates:

Extract and organize data into the candidates' database table.
Fields: id, First Name, Last Name, Current Title, Current Level, Current Company, Location, Current Job, Time at Current Job, Previous Positions, Current Operational Responsibilities, Current Strategic Responsibilities, Operational Responsibilities, Strategic Responsibilities, Undergraduate, Postgraduate, Skills, Key Skills Related to Tax/Finance, Projects, Achievements, Awards and Honors, Group Memberships, Causes, Interests, Tax Specialization, Links to Blog Posts, Articles, CPA, Certifications, Professional Associations, Tax Software Experience, Industry Experience, Languages, Experience.
Job Posts and Old Job Posts:

Extract and organize data into the job posts' database table.
Fields: id, Company Name, Role, Level, Salary, Salary Median, Location, State, Setting, In-State?, Industry, Public, Employee Count, Revenue, Benefits, Relocation, Undergraduate, Postgraduate, Experience, Field(s), CPA, Certifications, Strategic Responsibilities, Operational Responsibilities, Team Management, Budgetary Control, Decision-Making Authority, Reporting Structure, Cross-Functional Teams, Company Culture, Technology Proficiency, Stakeholder Engagement, Travel Requirements, Succession Planning, Crisis Management, Leadership Style, Change Management, Risk Management, Job Posting Source, Date Job Posted, Date Job Tracked, Works With Recruiters, Soft Skills, Hard Skills, Job Description Summary, Other Requirements.
Matching Function Training
The matching function will utilize OpenAI API intelligence and database information to improve over time. To optimize the matching results, we will use a hybrid search method that combines traditional keyword-based search with AI-driven semantic search. The app should intelligently consider various factors such as candidate experience, job requirements, and location preferences.

Development and Setup
The app will live in the "TS3000" folder on my desktop.
Create a virtual environment and ensure all dependencies are installed.
Remember, I am not a developer, so please guide me step-by-step through the process. Let's begin building this app to create an effective, optimized, and speedy system for matching candidates with jobs.