# pump_it_up

# CS4622-Machine-Learning-Project: Pump it Up: Data Mining the Water Table

Repository: https://github.com/chamikasudusinghe/pump_it_up

https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/

Competition Platform Infomation

username: moracse_170606e

BEST: 0.8202 (0.8225)

Rank: 1116 (669)

Model: CatBoost

# Methodology


### Handle Null Values

Null

<ol>
<li>public_meeting - replaced with mode</li>
<li>permit - replaced with mode</li>
<li>installer - replaced with mode</li>
<li>funder - replaced with mode</li>
<li>scheme_management - grouped with region_code and replaced</li>
<li>subvillage - grouped with region_code and replaced</li>
<li>scheme_name - grouped with region and replaced</li>
</ol>  

Zeros

<ol>
<li>gps_height - replaced with mean</li>
<li>amount_tsh - replaced with mean</li>
<li>num_private - replaced with mean</li>
<li>population - replaced with mean</li>
<li>construction_year - replaced with mean</li>
<li>corrdinates -  - replaced with mean</li>
</ol> 

### New Features

<ol>
<li>year_recorded - from data_recorded</li>
<li>no_of_years - from year_recorded - construction_year</li>
</ol>

### Removed Redundant Columns via Correlation

![image](https://user-images.githubusercontent.com/44718392/133864912-522f6410-e759-4fca-a9ef-d5f5e57e044f.png)

<ol>
<li>date_recorded</li>
<li>recorded_by</li>
<li>source_type</li>
<li>quantity_group</li>
<li>extraction_type_group</li>
<li>waterpoint_type_group</li>
</ol> 

### PCA

![image](https://user-images.githubusercontent.com/44718392/133864853-f9eed5cc-bbf9-415c-bbbd-768796e0603a.png)

explained_variance_ratio - 0.51618162, 0.2540258

### Training Accuracy

0.8899158249158249

### Feature Importance

![image](https://user-images.githubusercontent.com/44718392/133864939-eec76f09-a99d-4aad-b940-2a958ec625aa.png)

### Sharp Values

![image](https://user-images.githubusercontent.com/44718392/133864950-27df56f1-2243-4929-877d-c5516066232c.png)

![image](https://user-images.githubusercontent.com/44718392/133864957-cdddf315-8bd7-43c8-90e1-d7daefb1fbd8.png)

![image](https://user-images.githubusercontent.com/44718392/133864961-a5729ab3-d51f-417c-a0a4-2954b352d323.png)

![image](https://user-images.githubusercontent.com/44718392/133864963-5f658f57-d964-492e-94c5-dd0e29613ece.png)

### Results

![image](https://user-images.githubusercontent.com/44718392/133864980-53a08b6f-4f04-4b6c-b1c5-1b7963cdfe8b.png)

### Further explanation done in the notebook
