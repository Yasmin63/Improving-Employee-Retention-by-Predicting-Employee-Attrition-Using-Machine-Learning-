# Improving-Employee-Retention-by-Predicting-Employee-Attrition-Using-Machine-Learning

## Background
"Human resources (HR) is the main asset that needs to be managed properly by the company so that business goals can be achieved effectively and efficiently. On this occasion, we will face a problem about human resources in the company. Our focus is to find out how to keep employees to stay in the current company which can result in increased costs for employee recruitment and training for those who have just entered. By knowing the main factors that cause employee disengagement, companies can immediately address them by creating programs that are relevant to employee problems. "



## Data Preprocessing
- Drop Features. Drop features IkutProgramLOP, NomorHP and Email.
- Handling missing value. There are 6 features that have null value:
“IkutProgramLOP”  dropped
“AlasanResign” is fill with the mode value
“JumlahKetidakhadiran” is fill with the median value
“SkorKepuasanPegawai” is fill with the zero value
“JumlahKeikutsertaanProjek” is fill with the median value
“JumlahKeterlambatanSebulanTerakhir” is fill with the median value
- Handling Inconsistent.
“Product Design (UI & UX)” value in “AlasanResign” feature is replaced with “Dll”
“-” value in “StatusPernikahan” is replaced with “Belum_menikah”
“yes” value in “PernahBekerja” is replaced with “1”



## Annual Report on Employee Number Changes

![image](https://github.com/Yasmin63/Improving-Employee-Retention-by-Predicting-Employee-Attrition-Using-Machine-Learning-/assets/146631940/89808054-fe7f-48fe-8b26-90ee304accec)

Interpretation:
The growth in the number of employees occurred in the range of 2006 - 2018. In the 2013-2020 period, it appears that the company's condition is worrying because the number of employees continues to decrease until the peak occurred in 2018. This could be a sign that the company may be experiencing internal problems such as lack of growth opportunities, poor working environment, or financial problems.



## Resign Reason Analysis for Employee Attrition Management Strategy

![image](https://github.com/Yasmin63/Improving-Employee-Retention-by-Predicting-Employee-Attrition-Using-Machine-Learning-/assets/146631940/a11aecc3-09f4-4949-846b-59240dc42b6a)

Based on job position, Data Analyst has highest resignation rate (50%).

![image](https://github.com/Yasmin63/Improving-Employee-Retention-by-Predicting-Employee-Attrition-Using-Machine-Learning-/assets/146631940/4af6b369-849d-41b4-8bb7-f249f0aee246)

Interpretation:
All employees who resigned in the Data Analyst position were Fresh Graduate Program.
Recommendation:
The company can offer fresh graduate program employees more competitive benefits, conduct training, better self-development opportunities and create a more supportive work environment.

![image](https://github.com/Yasmin63/Improving-Employee-Retention-by-Predicting-Employee-Attrition-Using-Machine-Learning-/assets/146631940/24b2535c-e6a9-4f56-9f01-7613bd125fd8)

Interpretation:
Of the 8 Data Analyst employees who resigned, 2 of them had good performance and the other 4 were very good. This is certainly very detrimental to the company because the majority of employees who resign are employees with good performance.
Recommendation: 
The company can offer better salary, benefits and work-life balance to employees with good performance. In addition, the company is expected to offer good career paths and self-development to employees with good performance so that these employees feel valued and feel they will have a good career path in the company.

![image](https://github.com/Yasmin63/Improving-Employee-Retention-by-Predicting-Employee-Attrition-Using-Machine-Learning-/assets/146631940/ce5de649-6097-4f2f-8bc3-67aa9f18a770)

Interpretation:
Of the 8 employees, 6 Data Analyst employees resigned due to toxic culture and 2 resigned due to internal conflict. Both reasons illustrate that there are unfavorable factors from the internal position of the company's own Data Analyst.
Recommendation: 
The company can create an effective feedback system so that employees feel they can give input and receive constructive feedback. The company should also be able to resolve internal conflicts that occur between employees by facilitating meetings between employees to resolve problems. In addition, the company should re-evaluate the work culture and ensure that the culture is positive and motivates employees.



## Build an Automated Resignation Behavior Prediction using Machine Learning

- Handling outlier used z-score method
- Feature engineering. Create 3 new features: LamaBekerja, UsiaHiring, Resign
- Feature selection. Features that were removed: JenisKelamin, AlasanResign, TanggalPenilaianKaryawan, TanggalLahir, HiringPlatform
- Feature encoding. That feature were encoding: career, edu, performance
- Handling class imbalance. Feature resign
- Data train/test split and SMOTE
- Modeling

![image](https://github.com/Yasmin63/Improving-Employee-Retention-by-Predicting-Employee-Attrition-Using-Machine-Learning-/assets/146631940/ddcd1f70-656d-4da9-8f2d-d7e44b633360)

- ROC AUC

![image](https://github.com/Yasmin63/Improving-Employee-Retention-by-Predicting-Employee-Attrition-Using-Machine-Learning-/assets/146631940/da5363f7-17af-473e-b448-244a26bbe098)

- Confussion matrix

![image](https://github.com/Yasmin63/Improving-Employee-Retention-by-Predicting-Employee-Attrition-Using-Machine-Learning-/assets/146631940/b93ff643-8321-4146-a771-4f0814f288b3)



## Presenting Machine Learning Products to the Business Users

![image](https://github.com/Yasmin63/Improving-Employee-Retention-by-Predicting-Employee-Attrition-Using-Machine-Learning-/assets/146631940/08b51c88-9624-448e-8319-142bc187a9e5)

Interpretation:
It can be seen that “LamaBekerja” feature is the most important feature and is very dominant compared to other features in predicting the possibility of resigning from an employee. The SHAP value data shows that the smaller the length of service of an employee, the more likely the employee is to resign.
Recommendation: 
The company can review the existing corporate culture so as not to create a toxic work environment and hold a career development program to maintain employees, especially new employees who have good self-development potential. In addition, the company can also conduct surveys and ask for feedback from employees to understand their needs.
















