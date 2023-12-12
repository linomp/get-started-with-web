# Get Started with Web Applications
Simple path to get you started developing Web Applications.

The path covers HTML/CSS basics, APIs & how to quickly build one in Python, and makes you build a project on your own at the end. (everything free, from youtube)

_Tip:_ if you already have some background about APIs and websites, you can jump straight to the project and learn the stuff in a more natural order, completely based on need for advancing on the project. 

## (Optional) Git & Github

Check this [easy step-by-step lesson by Microsoft](https://github.com/microsoft/Web-Dev-For-Beginners/blob/main/1-getting-started-lessons/2-github-basics/README.md) and complete their checklist.

## The Path

**1. [How the world wide web works (12 min.)](https://youtu.be/guvsH5OFizE)** - Fundamental web application terms and context

  <img src="https://github.com/linomp/get-started-with-web/assets/40581019/5d9cf928-05a3-4c50-832e-7226b0ae754a" width="45%">

**2. [Frontend: Make a Website From Scratch (HTML & CSS) (2h)](https://www.youtube.com/watch?v=HXYZxVbWkjc&t=438s)** - Brad Traversy is the best Web Dev teacher on Youtube/Udemy. Here you will get a beginner-friendly intro to HTML & CSS, the mandatory basics of web. You will even deploy your project at the end!

   <img src="https://github.com/linomp/py-backend-path/assets/40581019/e385275f-7861-44c4-adb2-ad84960f0f60" width="45%">

**3. [Backend: Tutorial about APIs & FastAPI framework (58 min.)](https://www.youtube.com/watch?v=-ykeT6kk4bk&t=731s)** -  Learn backend concepts and create your first API with a modern & lightweight Python web framework.
  
   <img src="https://user-images.githubusercontent.com/40581019/175874893-8332d135-3306-490c-b6bd-671876d33d13.png" width="45%" />

**4. [Integration: FastAPI with Jinja2 templating engine (6 min.)](https://youtu.be/92iCfXAK0Gc?si=pb3YSVGmecCAa4jx)** - Learn to use a templating engine to make your FastAPI server return HTML views.

   <img src="https://github.com/linomp/py-backend-path/assets/40581019/26c20805-b504-4706-a39c-5cba4c5f77c0" width="45%" />

**5. Project Idea: Amazon price tracking app**

  Up to this point you should already have the building blocks down. You know how to create an API, how to create views with HTML & CSS and how to make the server return these views populated with dynamic data. 
  
  For this project you should create an app that allows you to input a url from a product on Amazon and a price threshold, and then it periodically scrapes the page to check the price and sends you an email when the price falls under the threshold.

  _Tip_: first focus only the API (the backend) and test with the Swagger UI. Later you can add an actual frontend, with the knowledge of steps 2 & 4.

  The API should have these endpoints:

  - POST `/tracking`: here I can send the url of a new product that I want to track and a price "threshold" for sending me an alert.
  - GET `/tracking`: returns me a list with the currently tracked product urls, along with product name, price threshold and best price so far.
  - GET `/config`: show me the email to which the alerts will be sent
    
## Further resources

### Web Scraping

- [Build amazon price tracking app (19 min.)](https://www.youtube.com/watch?v=Bg9r_yLk7VY). Does not build a web app, but contains all the steps for scraping AND sending you an email when the price is below a chosen threshold. 
  
  <img src="https://user-images.githubusercontent.com/40581019/175885423-704dfb3f-8d79-4704-bc1a-ccbb6cbcbcdb.PNG" width="45%" />

  _Note:_ The script created here runs only once. For monitoring the price automatically you will need to run it as a **Scheduled Task**, but it's easy. You could use the APScheduler library for that. This [answered stack overflow question](https://stackoverflow.com/questions/70104983/how-to-use-apscheduler-correctly-in-fastapi) shows how to do it (within FastAPI).

- [Web scraping with BeautifulSoup](https://www.youtube.com/playlist?list=PLzMcBGfZo4-lSq2IDrA6vpZEV92AmQfJK). 4 videos, from 11 to 27 mins. each.

  <img src="https://user-images.githubusercontent.com/40581019/175874933-a4f6a3d8-bfbb-4a15-ad80-394c039f57fb.PNG" width="35%" />

### Fullstack Applications (advanced)

If you want a more advanced frontend (with more complex interactions), you can learn a full-blown frontend framework like React.js (most popular one). This is how modern web applications are built nowadays.

- Start here: [React.js Beginner Tutorial (1h)](https://youtu.be/b9eMGE7QtTk?si=h3M9sY4RR0zl5Bb0)
- Then: [How to build a React + FastAPI application (1h)](https://www.youtube.com/watch?v=0zb2kohYZIM)
  
