# Developing APIs with Python

Stripped down path to teach you what are APIs, how to build one quick with FastAPI (that also follows modern best practices), and makes you build a project on your own at the end.

## Git & Github

Check this [easy step-by-step lesson by Microsoft](https://github.com/microsoft/Web-Dev-For-Beginners/blob/main/1-getting-started-lessons/2-github-basics/README.md) and complete their checklist.

## The Path

**0. [How the world wide web works (12 min.)](https://youtu.be/guvsH5OFizE)** :mortar_board:: elemental web application terms and context

  <img src="https://github.com/Tar-Baby/py-backend-path/assets/40581019/72eacfb2-a203-4b9d-a35e-435ac20af435" width="45%">

**1. [Tutorial about APIs & FastAPI framework (58 min.)](https://www.youtube.com/watch?v=-ykeT6kk4bk&t=731s)** - TechWithTim makes the best python videos.
  
   <img src="https://user-images.githubusercontent.com/40581019/175874893-8332d135-3306-490c-b6bd-671876d33d13.png" width="45%" />

**2. [Build amazon price tracking app (19 min.)](https://www.youtube.com/watch?v=Bg9r_yLk7VY)**  - you don't build a web app, but contains all the steps for scraping AND sending you an email when the price is below a chosen threshold. 
  
   <img src="https://user-images.githubusercontent.com/40581019/175885423-704dfb3f-8d79-4704-bc1a-ccbb6cbcbcdb.PNG" width="45%" />

**3. Project Idea:** Use the knowledge from steps 1 & 2 to build an API with these endpoints:
  - POST `/tracking`: here I can send the url of a new product that I want to track and a price "threshold" for sending me an alert.
  - GET `/tracking`: returns me a list with the currently tracked product urls, along with product name, price threshold and best price so far.
  - GET `/config`: show me the email to which the alerts will be sent
    
    Notes: 
    - First focus only the API (the backend). Later you can investigate how to add an actual UI / web page (the frontend).
    - also, the script created in step 2 runs only once. For monitoring the price automatically you will need to run it as a **Scheduled Task**, but it's easy. This [answered stack overflow question](https://stackoverflow.com/questions/70104983/how-to-use-apscheduler-correctly-in-fastapi) shows how to do that (within FastAPI).

## Further resources

#### More about Web Scraping
- [TechWithTim: Web scraping with BeautifulSoup](https://www.youtube.com/playlist?list=PLzMcBGfZo4-lSq2IDrA6vpZEV92AmQfJK). 4 videos, from 11 to 27 mins. each.

  <img src="https://user-images.githubusercontent.com/40581019/175874933-a4f6a3d8-bfbb-4a15-ad80-394c039f57fb.PNG" width="35%" />

#### More about Web Applications
- [Fullstack development tutorial (1h)](https://www.youtube.com/watch?v=OzUzrs8uJl8). Learn to connect FastAPI (backend), ReactJS (frontend) and MongoDB (database) by building a To-Do list app.
  
- [Learn HTML & CSS building a portfolio website (2h)](https://youtu.be/r_hYR53r61M). Responsive layout, browser local storage (chosen theme persists after page refresh).
 
  <img src="https://user-images.githubusercontent.com/40581019/133420469-aa1fb07e-2ff7-4eed-8047-e3702c3dc316.PNG" width="35%" />
