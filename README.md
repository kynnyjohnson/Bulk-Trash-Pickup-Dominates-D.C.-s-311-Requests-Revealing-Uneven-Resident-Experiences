# kyns-final
**DC 311 Service Requests Analysis**

**Overview**
This project analyzes Washington, D.C. 311 service request data from 2025 to examine what kinds of city service issues residents reported, which agencies handled them, and how quickly cases were resolved. Looking at service request patterns can help show what problems appear most often in the city and whether response times vary depending on the type of complaint or service requested. This matters because 311 data offers a public record of how residents interact with city services and how local governments respond to quality-of-life concerns.

**Data Sources**
The data comes from Washington, D.C.’s 311 service request records. The raw dataset originally contained 440,601 rows. It includes fields such as service request ID, street address, service code, service description, agency, add date, resolution date, service order status, priority, and ward. After cleaning and narrowing the data for analysis, the final cleaned dataset contained 4,324 rows.

**Methodology**
I began with the raw 311 dataset, which originally contained 440,601 rows, and cleaned it to make the data easier to analyze. I standardized column names, reviewed missing and inconsistent values, and focused on the variables most relevant to reporting, including service request ID, service code description, organization acronym, add date, resolution date, service order status, and ward. I converted date fields into a consistent format and used them to calculate resolution time where both an add date and resolution date were available. I also filtered the dataset down to the records most relevant to my reporting focus, which resulted in a cleaned working file of 4,324 rows. From there, I grouped requests by service type, agency, and ward to identify patterns in the data and reviewed statuses such as Closed, In-Progress, Canceled, and Closed (Duplicate) to avoid treating all records the same in the analysis.

**Limitations**
This dataset cannot explain why some neighborhoods generate more requests than others, since it does not include population size, reporting behavior, or broader neighborhood context. It also cannot show whether a resident was satisfied with the response, only whether a request received a status update. Because the original dataset was reduced from 440,601 rows to 4,324 rows for the purposes of this project, the cleaned file reflects a narrower slice of the full dataset rather than the entire universe of 311 requests. Some records also contain missing values or unusual timelines that may reflect administrative processes rather than actual service delays.
