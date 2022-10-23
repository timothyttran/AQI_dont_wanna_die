# AQI_dont_wanna_die

## Inspiration
On October 20th, Seattle made headlines, having the worst air quality in the world.

Living in Seattle, our hackathon team felt some of the effects firsthand, from teary eyes to sore throats as we walked to our classes.

We decided to build a project to address this very relevant issue.

## What it does
AQI Don't Wanna Die is a web application featuring a ML model to determine if  the surrounding air quality is "dangerous" for your health.

Unlike the traditional AQI scale, AQI Don't Wanna Die takes in various inputs (humidity, temperature, air pressure, etc.) to output a binary result. The result of "safe" or "unsafe" is arguably more straightforward than the numerical AQI scale for ordinary citizens.

Moreover, AQI Don't Wanna Die offers a potentially more standardized alternative than simply looking up AQI results online since many sources provide conflicting numbers. With this tool, you can input your own information to get a trusted result.

We also incorporated a chatbot (courtesy of Google Cloud/Dialog Flow) to recognize when a user inputs statements that may pertain to their health. Then, the chatbot responds about how these statements should be interpreted with regards to air pollution safety.

## How we built it
The website we built is based on a boilerplate Bootstrap template, although we significantly customized the site with animations, new layouts, and other styling components.

We created the ML model using Python and Sci-Kit Learn with a SVM. Our data originated from a Kaggle dataset about fire alarms. To deploy the model, we used Streamlit.

The chatbot was built with Dialog Flow by Google Cloud.
