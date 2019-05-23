# Terminology
This specification uses the terms **MUST,SHOULD,MAY,MUST NOT, MAY NOT, SHOULD NOT,RECOMMENDED,OPTIONAL** as defined in RFC 2119[frc2119] and BCP 141. We also use the following terminology to specify the user states. When the following words are captialized or in the name of message types, they have specific defined meaning as follow:

**WECHAT LOGIN:** Login through wechat api.  
**UCL LOGIN:** Login through ucl.  
**GUEST:** Neither use WECHAT LOGIN nor  use UCL LOGIN.  
**USER:** Either WECHAT LOGIN or UCL LOGIN.
**LOCAL TIMEZONE:** GMT0
**LOCAL CITY:** London
**UCL:** University College London
**CSSA:** UCL Chinese Students and Scholars Association 

# Functional Requirments   
## Main Page  
### Weather and Date  
This part should contain two parts Date and the Weather. We use LOCAL TIMEZONE and LOCAL CITY.
#### Weather Desciption  
Format: Weather + Highest Degree(Celsius) + Lowest(Celsius) + Suggest dressing  

## News  
News are displayed inside a scroll bar with speed 2s/time(Every two seconds scroll to the left once).  
### Content  
This MUST contain CSSA activities. MAY contain other information if required.  
### Scroll Bar   
Scroll Bar SHOULD display pictures, each pictures represent an article.  



