# Ocean-Skill-Dashboard-Development

**Objective**

To automate data integration and transformation processes in Power BI for the I&D Ocean Compliance Dashboard, ensuring accurate and efficient monthly updates without manual intervention.
#

**Automation Overview** <br>

**File Automation:** <br>
Automates file management tasks like loading, refreshing, and updating data sources without manual effort, using scheduled refresh and logic-driven updates in Power BI.

**Data Sources Automated** <br>

**Employee Master:** <br>
Latest file is auto-loaded and refreshed in Power BI. <br>
**Employee GAD (Previous):** <br>
Second latest file is refreshed automatically without manual updates. <br>
**I&D Ocean (Current):** <br>
Current data file is refreshed automatically and processed for reporting.<br>
**I&D Ocean (Previous):** <br>
Second latest I&D Ocean file follows the same automation and transformation rules. <br>
#
**Power Query Transformations**

**1. Column Renaming** <br>
Updated terminology to align with dashboard standards. <br>
**Examples:** <br>

“Global Employee Id” → “Global Emp Id” <br>
“Attempt 1 Score” → “Technology Score Attempt 1” <br>
“SkillSet” → “Track” <br>
 (All changes are included in the documentation)
#

**2. Fill Down Operation** <br>
Blank/null cells in key columns (e.g., Role, Assessment Status, Score Bucket) are filled with the value from the row above for consistency. <br>

**3. Grouped Rows** <br>
Replaced the “Certified” column with a more standardized “Certification Status” for grouped data views<br>

# 

**Maintenance Requirement** <br>

All transformation steps applied to the Current I&D Ocean data must also be mirrored in the Previous file every month to maintain dashboard consistency and accuracy.
