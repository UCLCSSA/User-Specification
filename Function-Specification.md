# 1.Terminology
This specification uses the terms **MUST,SHOULD,MAY,MUST NOT, MAY NOT, SHOULD NOT,RECOMMENDED,OPTIONAL** as defined in RFC 2119[frc2119] and BCP 141. We also use the following terminology to specify the user states. When the following words are captialized or in the name of message types, they have specific defined meaning as follow:

**WECHAT LOGIN:** Login through wechat api.  
**UCL LOGIN:** Login through ucl.  
**GUEST:** Neither use WECHAT LOGIN nor  use UCL LOGIN.  
**USER:** Either WECHAT LOGIN or UCL LOGIN.  
**LOCAL TIMEZONE:** GMT0  
**LOCAL CITY:** London  
**UCL:** University College London  
**CSSA:** UCL Chinese Students and Scholars Association 

# 2.Functional Requirments   
## 2.1 Main Page  
### 2.1.1 Weather and Date  
This part should contain two parts Date and the Weather. We use LOCAL TIMEZONE and LOCAL CITY.
#### 2.1.1.1 Weather Desciption  
Format: Weather + Highest Degree(Celsius) + Lowest(Celsius) + Suggest dressing  

## 2.2 News  
News are displayed inside a scroll bar with speed 2s/time(Every two seconds scroll to the left once).  
### 2.2.1 Content  
This MUST contain CSSA activities. MAY contain other information if required.  
### 2.2.2 Scroll Bar   
Scroll Bar SHOULD display pictures, each pictures represent an article.  
### 2.2.3 When User press picture on the scroll bar  
Full article SHOULD be displayed in a new page  

## 2.3 Personal Timetable(todo What if in GUEST mode) 
This part contains two components:

1. Scroll bar which displays today's lectures  
2. Button called "显示完整课表" in the bottom  

Each lecture is displayed inside a block. The Scroll bar only move when user scroll it.  
### 2.3 Block  
This SHOULD include following information:  

1. Start and End Time (1)  
2. Lecture Room (2)  
3. Lecture Name (3)  
4. Lecture Format[Lecture, Problem Base Learning, Tutoring] (4)  

-------------------------
|    |                  |
-    |-------------------
| (1)|                  |
-    |-------------------
|    |                  |
-----|-------------------