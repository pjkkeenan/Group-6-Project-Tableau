# MIST-PROJECT-2
MIST 4610 - Project 2 

<h1>TEAM MEMBERS (21484_G6)</h1>
<li>Ademoye, Adekanle <a href="https://github.com/ata-uga">ata-uga</a></li>
<li>Keenan, Patrick <a href="https://github.com/pjkkeenan">pjkkeenan</a></li>
<li>Patel, Kishan <a href="https://github.com/kp0024">kp0024</a></li>
<li>Thomas, Reuben <a href="https://github.com/Reubenuga">rmt08737</a></li>
<li>Patel, Nidhi <a href="https://github.com/ndp88405">ndp88405</a></li>

<h1> Dataset Description </h1>
<p>The data was obtained from the Data Catalog of the US Government. The dataset contains 14365 rows representing different individuals and their families, with the columns representing various information about them. The following data contains the text datatype. Some of these have numeric values in them, but that number represents a categorical value, a value that is used to group data into categories, rather than a quantitative value. The data that covered Ethnicity was split into two columns: the name of each ethnicity and an ethnicity code with a number representing the ethnicity. The number is to aid in the ease of viewing and understanding. Geographic Unit is another set of data that was split into columns. This time it is in 3 columns: Geotype, which stands for the Type of Geographic Unit, and distinguishes between Neighborhood, Census Tract, Place, Zipcode, County, and Region. Geotype wasn’t an interesting dataset as it was all mainly grouped into counties, with no other type appearing. The other two types were Geotypevalue, which is the value of the geographic unit that contains the zipcodes, and Geoname, which names each of the counties.</p>
<p>This set of data is very redundant as there is already a column specifically for the county names called County_name. The next is County_FIPS. FIPS stands for Federal Information Processing Standard code. This is a numeric code that is used to identify states and counties to aid in data collection and analysis. The next is Region_Name, which is used to differentiate between different areas in California, such as the San Joaquin Valley or the Bay Area, for example. The next is Region_Code, which assigns a numeric value to each of the region names to aid in data analysis. The following data contains the numerical datatype. Cost_yr is our first numerical/ quantitative data type, and it represents the annual food costs that each family incurs. Next is median_income, which represents the family’s median income. Then we have two columns that seem similar, which are affordability_ratio and CA_RR_Affordability. Affordability ratio is the ratio of food cost as compared to income. CA_RR_Affordability compares the affordability ratio of a county to the California average. We then have LL_95CI, which is the Lower limit of the 95% Confidence Interval, which means that under repeated sampling, the value that we are testing for will fall within the lower part of the data, 95% of the time. The UL_95CI is just the same, but for the Upper Limit. SE_food_afford is the Standard Error, which is how much the sample data may differ from the true population data. Then we have RSE_food_afford, which is the Relative standard error, which means how precise an estimate is relative to the size of the estimate. So if the RSE is high, then it means it is not very precise and vice versa. The Food_afford_decile is the statewide decile ranking, which is labeled as a numeric data type but is described as essentially a ranking where each county is given a rank based on the food affordability ratio. Lastly, we have ave_fam_size, which is the average family size. </p>



<h1> Questions (2) </h1>

<ol>1. Which counties in California have the lowest food affordability ratios, and how does that relate to their median income levels?</ol>
<ol>2. Do racial and ethnic disparities in food affordability vary between the Bay Area and San Joaquin Valley in California during the 2006-2010 period?</ol>
<h4>Question 1 Importance</h4>
<li>Economic Importance:</li>
<p>Identifying counties with the worst food affordability highlights regions where residents are most financially burdened. This can inform government resource allocation (such as food assistance programs, minimum wage policies, or local subsidies).</p>
<li>Social Importance:</li>
<p>Food insecurity often leads to poor health outcomes, higher stress, and reduced educational performance. Highlighting counties where food affordability is worst helps target community health interventions.</p>
<li>Cultural Importance:</li>
<p>When food becomes unaffordable, culturally significant foods might be substituted with cheaper, less healthy alternatives. This can erode cultural food traditions and community identity.</p>
<h4>Tied to Datasets</h4>
<li>The food affordability ratios are directly mentioned in the Data Dictionary and would typically be measured from surveys like the USDA's or Feeding America's food insecurity studies.</li>
<li>Median income data for each county during 2006–2010 is tied to the American Community Survey (ACS) 5-Year Estimates, referenced in your dataset documentation.</li>
<li>County-level mapping from the "MPO-CountyList" sheet allows linking affordability outcomes with specific counties.</li>
<h4>Question 2 Importance</h4>
<li>Social Importance:</li>
<p>Examining racial and ethnic disparities addresses social justice concerns. If certain racial/ethnic groups systematically face worse food affordability, that reflects systemic inequality requiring policy solutions.</p>
<li>Economic Importance:</li>
<p>Food affordability directly impacts wealth building and economic opportunity. Addressing disparities can help close economic gaps between racial and ethnic groups.</p>
<li>Cultural Importance:</li>
<p>Access to culturally appropriate foods is key to preserving the identity and traditions of minority groups. Lack of affordability for these foods can have long-term cultural consequences.</p>
<h4>Tied to Datasets</h4>
<li>Race/ethnicity breakdowns (race_eth_code, race_eth_name) are explicitly listed in the Data Dictionary.</li>
<li>Regional grouping (Bay Area vs. San Joaquin Valley) can be constructed using the "MPO-CountyList," which connects counties to broader regions.</li>
<li>The 2006–2010 time frame matches the reporting years stated in your metadata, ensuring the findings align with the historical context.</li>


<h1> Analysis and Results </h1>

<h2>Question 1 Visualization</h2>
<img width="650" src ="https://github.com/user-attachments/assets/07e94884-a045-4bf2-8861-26a079b11456">
<li>Counties with lower median incomes tend to have higher affordability ratios.</li>
<li>This indicates that in many counties, food consumes a larger portion of income. </li>
<li>San Mateo County has a high food affordability ratio due to factors such as high population density and a homelessness problem that weighs down median income among other socioeconomic factors that further contribute to this problem</li>

<h2>Question 2 Visualization</h2>
<img width="650" src ="https://github.com/user-attachments/assets/1fc14b39-67bb-47ca-85a3-c8deb4e25900">
<li>San Joaquin Valley shows greater disparities across ethnic groups.</li>
<li>African American and Latino populations face higher affordability burdens, which makes it more expensive.</li>
<li>Regional economic and housing differences likely contribute.</li>
<li>Bay Region has a higher cost of living compared to San Joaquin Valley</li>
<li>Since San Joaquin is primarily an agricultural area, the primary workforce is made up of farmers, who have lower incomes than those in the Bay Area, which leads to a higher affordability ratio 
</li>

<h1> Tableau Packaged Workbook </h1>

<ul><a href="https://raw.githubusercontent.com/ndp88405/MIST-PROJECT-2/refs/heads/main/new%20california%20heat%20map%20woorkbook%20with%20avg%20income.twbx">Question 1</a></ul>
<ul><a href="https://raw.githubusercontent.com/ndp88405/MIST-PROJECT-2/refs/heads/main/Project%202%20-%20Question%202.twbx">Question 2</a></ul>

[new corrected wookbook for question 1.zip](https://github.com/user-attachments/files/19964656/new.corrected.wookbook.for.question.1.zip)

