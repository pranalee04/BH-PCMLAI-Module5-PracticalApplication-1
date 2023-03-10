# Module5-PracticalApplication-1
This repository is the solution for practical assignment 1 for Module 5 of the BH-PCMLAI course. The goal is to find the answers to the question, “Will an Amazon customer accept the coupon?” based on the UCI Machine Learning repository created via a survey on Amazon Mechanical Turk.

## Will a Customer Accept the Coupon?

Please use the link  [prompt.ipynb](https://github.com/pranalee04/BH-PCMLAI-Module5-PracticalApplication-1/blob/main/assignment_5_1_starter/prompt.ipynb) to access the assignment 5.1

------

**Context**

Imagine driving through town and a coupon is delivered to your cell phone for a restaraunt near where you are driving. Would you accept that coupon and take a short detour to the restaraunt? Would you accept the coupon but use it on a sunbsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaraunt? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

------
**Overview**

The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

------
**Data**

This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’.  There are five different types of coupons -- less expensive restaurants (under \\$20), coffee houses, carry out & take away, bar, and more expensive restaurants (\\$20 - \\$50). 

------
### Data Description
Keep in mind that these values mentioned below are average values.

The attributes of this data set include:
1. User attributes
    -  Gender: male, female
    -  Age: below 21, 21 to 25, 26 to 30, etc.
    -  Marital Status: single, married partner, unmarried partner, or widowed
    -  Number of children: 0, 1, or more than 1
    -  Education: high school, bachelors degree, associates degree, or graduate degree
    -  Occupation: architecture & engineering, business & financial, etc.
    -  Annual income: less than \\$12500, \\$12500 - \\$24999, \\$25000 - \\$37499, etc.
    -  Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    -  Number of times that he/she buys takeaway food: 0, less than 1, 1 to 3, 4 to 8 or greater
    than 8
    -  Number of times that he/she goes to a coffee house: 0, less than 1, 1 to 3, 4 to 8 or
    greater than 8
    -  Number of times that he/she eats at a restaurant with average expense less than \\$20 per
    person: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    -  Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
    

2. Contextual attributes
    - Driving destination: home, work, or no urgent destination
    - Location of user, coupon and destination: we provide a map to show the geographical
    location of the user, destination, and the venue, and we mark the distance between each
    two places with time of driving. The user can see whether the venue is in the same
    direction as the destination.
    - Weather: sunny, rainy, or snowy
    - Temperature: 30F, 55F, or 80F
    - Time: 10AM, 2PM, or 6PM
    - Passenger: alone, partner, kid(s), or friend(s)


3. Coupon attributes
    - time before it expires: 2 hours or one day

## File structure

The project file structure is as follows:

- The jupyter notebook.
- data folder for the dataset.
- images for charts.

## Overall Analysis

1. Coffee House coupons were most accepted, followed by cheap Restaurant and Carry out; Bar coupon acceptance was only 11.5 %. Expensive restaurant coupons were least accepted
2. People under 30 accepted more coupons. 
3. Females accepted more Coffee House coupons while Males accepted more Bar cupon, however, Take out or Carry Away and both genders almost equally accepted cheap restaurants
4. Percentage of people who don't have kids have an income less than 50k, are younger than 30 years, and visit cheap restaurants will accept a coupon for bars 15.73 % times
5. The likelihood people age under 35 also accepts other types of coupons is high if they earn a salary of less than 50k and don't have kids. 
6. Percentage of people who went to Bar under 3 days 81.34517766497463 %
7. Percentage of people who went to Bar more than 3 days 18.654822335025383 %
8. People who visit Bar less than 3 and in the range of 4 to 8 are more likely to accept the coupon. Interestingly people who visit bar often are less likely to take the coupon
9. The acceptance rate among people who go to a bar more than once a month and are over the age of 25 is 70.92 %
10. The acceptance rate among people who go to a bar more than once a month and are under the age of 25 is 29.08 %
11. Percentage of people who are not Kids and  Widowed and go to Bar is 95.92 %
12. People who go to bars more than once a month and are under the age of 30 is 60.20 %
14. People who go to cheap restaurants more than 4 times a month and their income is less than 50K is 48.25 %.


 ### Next Steps and Recommendations
 - Need more data on Car column

------


