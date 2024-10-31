# TDS_Project1

This project collects detailed information about Github users in Sydney with over 100 followers and up to 500 of their most recent repositories. The data includes various user demographics and activity statistics, providing insights into the community of developers on Github in Sydney. Findings reveal trends and suggest actionable advice for developers and organizations based on user and repository data.

##Data Collection Process
Data was collected using the Github REST API to retrieve user and repository information:

###Users Information: 
We fetched details for Sydney-based Github users with over 100 followers, including their basic profile, company, contact information, and activity metrics. After retrieving the raw data, the company field was standardized:

 - Trimmed of any extra whitespace.
 - Stripped of any leading "@" symbol (only the first one).
 - Converted to uppercase for consistency.

###Repositories Information: 
For each user, we collected up to the 500 most recent public repositories. The following details were retrieved:

 - Repository metadata (name, creation date, language, stars, and watchers).
 - Specific features like whether the repository supports projects or a wiki.
 - License details (license name under license.key).

##Interesting and Surprising Findings
One particularly surprising finding was that a significant percentage of repositories lacked essential README files and clear documentation, even for users with high follower counts. This could indicate that while Sydney developers are active on Github, some foundational repository practices are being overlooked, especially among users with a high volume of projects.

##Actionable Recommendation
To improve the visibility and usability of repositories, developers should focus on adding well-structured READMEs and clear documentation to their projects. A quality README with installation instructions, usage examples, and license information can significantly boost repository engagement. Additionally, organizations may encourage documentation practices as part of their open-source initiatives to support new contributors.
