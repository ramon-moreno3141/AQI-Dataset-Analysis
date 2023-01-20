# AQI-Dataset-Analysis
<strong>Files Worked On: AQI.pdf (A printout of the python code and analysis done on jupyter notebook)</strong><br>

<strong>Description:</strong> An analysis on AQI data for the year 2020 from USA EPA data. The analysis investigates how AQI various both geographically and over time
and predicts AQI at certain points in time for various locations in California. The project demonstrates EDA (exploratory data analysis), merging on locations using
Pandas, interpolation techniques, and different visualizations used to represent the data. The
names of the different data files used are listed in Section 1.5 (Page 2).

<strong>Highlights:</strong><br>
<ul>
  <li><strong>Section 1.5.2 (Page 3):</strong> Day and month columns were added to the <em>daily_county_aqi</em> table to make it easier to perform a time analysis on the data. The day and month columns were extracted from an already existing 'Date' column.</li>
  
  <li><strong>Section 1.5.3 (Page 4):</strong> All the tables used in the project were filtered to only include <strong>daily data</strong> in the state of California. This would make it easier to do a focused analysis on AQI levels in California.</li>
  
  <li><strong>Section 1.5.4 (Page 4 and 5):</strong> The <em>daily_county_aqi</em> table was left merged with the <em>aqs_sites</em> table in order to get the latitude and longitudes of each of the measurements in the <em>daily_county_aqi</em> table.</li>
  
  <li><strong>Section 1.5.5 (Page 6):</strong> Unneeded columns were removed from the <em>traffic_data</em> table and an 'AADT' column was added where the values were calculated from other columns in the table. Illegal values were cleaned or replaced using methods such as <strong>.strip()</strong> or <strong>.replace()</strong>.</li>
  
  <li><strong>Section 1.5.6 (Page 7):</strong> The tables <em>traffic_data_cleaned</em> and <em>epa_data_CA_merged</em> were joined into a geopandas dataframe using the geopandas package. A spatial join was used to match the <em>epa_data_CA_merged</em> rows with the row in <em>traffic_data</em> that it is the "closest" to.</li>
  
  <li><strong>Sections 1.6.1 and 1.6.2 (Pages 8-10):</strong> The states with the top 10 worst average median AQIs and the top 10 worst average max AQIs were calculated as shown on page 9. Section 1.6.2 on page 10 analyzes why some of these states are on these lists. States such as California, Arizona, and Nevada are in the southwestern part of the United States which is dry due to the topographical differences that prevent moisture from reaching these regions.</li>
  
  <li><strong>Section 1.6.4 (Pages 11-12):</strong> On page 11, the number of dates with missing AQI information is calculated for each county in California. Each county in California is then mapped to a list of the dates with missing AQI information. Question 4bii on page 12 analyzes key missing dates in common between the counties and also explores why certain counties have the most missing days.</li>
  
  <li><strong>Sections 1.7.2 and 1.7.3 (Pages 19-23):</strong> Various visualizations to represent the data are created in Section 1.7.2 on page 19 and shown on pages 20-22. The data used for the visualizations was manipulated prior in section 1.7.1 on page 18. A summary of the findings and visualizations is in section 1.7.3 on page 23.</li>
</ul>
