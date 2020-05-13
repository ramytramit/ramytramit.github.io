---
layout: project
type: project
image: images/snackademic_logo1.png
title: Snackademic: A Site to Satiate Your Manoa Munchies
permalink: projects/snackademic
# All dates must be YYYY-MM-DD format!
date: 2020-05-12
labels:
  - Semantic UI
  - React
  - Meteor
  - Mongo DB

summary: A website made for the final project in my ICS 314 class, Spring 2020.
---

## Snackademic: A Site to Satiate Your Manoa Munchies

## Table of Contents
* [Overview](#overview)
* [Goals](#goals)
* [Team](#team)
* [Project Progress & Development History](#project-progress--development-history)
* [Mockup](#mockup)
* [Galaxy Deployment](#galaxy-deployment)
* [Developer Guide](#developer-guide)
* [Quality Assurance](#quality-assurance)
* [User Guide](#user-guide)
* [Community Feedback](#community-feedback)
* [Future Improvements](#future-improvements)


### Overview
The goal of Snackademic is to give students at UH a way to keep track of all their favorite foodtrucks and restaurants across campus, see what their menu offerings are, filter by style of food, and see what hours they are open. In the case of foodtrucks, the app will let the student view exactly where on campus they are located for the day. The app will also let UH students rate their favorite restaurants by creating user profiles. User profiles can also be created for restaurants and admins.

The app will be built utilizing [Semantic UI React](https://react.semantic-ui.com/), [Meteor](https://www.meteor.com/), [React](https://reactjs.org/), and [Uniforms](https://uniforms.tools/). Details on how to install and run the application locally will be provided soon.


### Goals:
  * Create a website where students can go to see what food is available, including pages for the following:
    * Food Trucks
    * Resturants/Dining Halls
    * Menus
    * Hours
    * Locations
  * Provide a place to review these food places
    * Written Review individual locations
    * 1-5 star feedback


### Team:
Please feel free to contact any of us via our GitHub links provided below. You may also view our GitHub organization page here: [github.com/the-back-corner](https://github.com/the-back-corner)
* [Clark Whitehead](https://clark-whitehead.github.io)
* [David Harris](https://devoider.github.io)
* [Jasmine Singleton](https://jrsingleton.github.io)
* [Ramit Islam](https://ramytramit.github.io)


### Project Progress & Development History
You can follow the team's progress via our Milestones here:
* [M1](https://github.com/the-back-corner/snackademic/projects/1)
* [M2](https://github.com/the-back-corner/snackademic/projects/2)
* [M3](https://github.com/the-back-corner/snackademic/projects/3)


### Mockup:

![](images/mockup.png)


### Galaxy Deployment:
You can view our deployed page on Galaxy here: <del>[snackademic.meteorapp.com](http://snackademic.meteorapp.com/)</del>

**UPDATE:** Since our trial run on Galaxy has expired, we have updated all the images for our site to reflect what you'd see if the site were active.

**Landing Page**

![](images/landing.png)


### Developer Guide
This section provides information of interest to Meteor developers wishing to use this code base as a basis for their own development tasks.

#### Installation
First, [install Meteor](https://www.meteor.com/install).

Second, visit the [snackademic application github page](https://github.com/the-back-corner/snackademic), and click the "Use this template" button to create your own repository initialized with a copy of this application. Alternatively, you can download the sources as a zip file or make a fork of the repo.

Third, go to your newly created repository, and click the "Clone or download" button to download your new GitHub repo to your local file system.  Using [GitHub Desktop](https://desktop.github.com/) is a great choice if you use MacOS or Windows.

Fourth, cd into the app/ directory of your local copy of the repo, and install third party libraries with:

```
$ meteor npm install
```

#### Running the system

Once the libraries are installed, you can run the application by invoking the "start" script in the [package.json file](https://github.com/ics-software-engineering/meteor-application-template-react/blob/master/app/package.json):

```
$ meteor npm run start
```

The first time you run the app, it will create some default users and data. Here is the output:

```
meteor npm run start

> meteor-application-template-react@ start /Users/philipjohnson/github/ics-software-engineering/meteor-application-template-react/app
> meteor --no-release-check --settings ../config/settings.development.json

[[[[[ ~/github/ics-software-engineering/meteor-application-template-react/app ]]]]]

=> Started proxy.
=> Started MongoDB.
I20180227-13:33:02.716(-10)? Creating the default user(s)
I20180227-13:33:02.742(-10)?   Creating user admin@foo.com.
I20180227-13:33:02.743(-10)?   Creating user john@foo.com.
I20180227-13:33:02.743(-10)? Creating default data.
I20180227-13:33:02.743(-10)?   Adding: Basket (john@foo.com)
I20180227-13:33:02.743(-10)?   Adding: Bicycle (john@foo.com)
I20180227-13:33:02.743(-10)?   Adding: Banana (admin@foo.com)
I20180227-13:33:02.744(-10)?   Adding: Boogie Board (admin@foo.com)
=> Started your app.

=> App running at: http://localhost:3000/
```

### Quality Assurance

#### ESLint

The application includes a [.eslintrc](https://github.com/ics-software-engineering/meteor-application-template-react/blob/master/app/.eslintrc) file to define the coding style adhered to in this application. You can invoke ESLint from the command line as follows:

```
[~/meteor-application-template-react/app]-> meteor npm run lint

> meteor-application-template-react@ lint /Users/philipjohnson/meteor-application-template-react/app
> eslint --quiet ./imports
```

ESLint should run without generating any errors.

It's significantly easier to do development with ESLint integrated directly into your IDE (such as IntelliJ).


### User Guide
#### To get started with our application, please follow the steps outlined below.

* First, **Register** for an account by clicking the Register button on the main landing page or from the dropdown page on the top right of the nav bar. Your password must be at least 8 characters.

![](images/register.png)


* If you have already registered, **Sign In** by clicking the Sign In button on the landing page (or from the drop down menu on the top right corner of the nav bar). You'll then be redirected to the Sign In page as depicted in the image below. For this example, we will log in as as a "user" given the default sign in credentials for the class. You will be redirected to a different page based on the role of your account.

![](images/signin.png)

* On the account page, you can see your favorite restaurants, reviews, and your user account information.

![](images/accountpage.png)

* You can change your password

![](images/change-password.png)

* Or deactivate your account

![](images/delete-account.png)

* You can select a foodtruck or restaurant from the dropdown, and it will redirect to

![](images/restaurants.png)

* You can add it to favorites, by clicking the add to favorites button.

![](images/remove-favorite.png)

* View the menu

![](images/foodtrucks.png)

* View the reviews (currently the only page with reviews is Sistahs foodtruck)

![](images/review-preview.png)

* The Maps page displays where the restaurants and foodtrucks are currently, and when they are open. If it is tuesday it will display this:

![](images/maps.png)

* The Hours page displays the hours of each restaurant/foodtruck hours depending on the day, if it is Tuesday it will display this:

![](images/hours.png)

* As a Vendor, you can view your eatery

![](images/vendoreatery.png)

* As an Admin, you can view the registered accounts:

![](images/allaccounts.png)

### Community Feedback

We asked several members of the community to test out our application and give us some feedback on it. A few updates to the app were made based on their evaluation. These changed included things such as unifying the aesthetics and colors, and updating some of our button functionalities and background images. The summary of their assessments are as follows:

* **Test User 1:**  The visual is 10/10, but the menu leaves something to be desired. Some pages look a bit odd in regards to scaling and placement. Footer doesn't stick to the bottom of my browser, and data takes forever to load. Overall, I would give it a 9/10. It's definitely a project to be proud of. ~ Lianphain

* **Test User 2:**  The site is generally aesthetically pleasing, but the white text of the restaurant descriptions is a bit hard to read against many of the background images.  It's not terrible, but you have to put some effort into reading it which is more than preferable.  Being able to see menu items, prices, locations, and hours is very convenient, but it would be nice if it was more interlinked.  Being able to see hours (or at least today's hours) and location on the restaurant page would have been nice.  It would have been nice if the map was more dynamic, such as taking you to a restaurant page when you clicked on the corresponding icon, though I know that would have been a lot harder to implement (and also google maps integration costs money now, right?  I fully understand it wouldn't have been worth it for a school project, if I'm trying to review outside that context, it would have been nice to see. Overall, despite my criticisms, it's quite a nice site.  It's just easier to note the things that could have been better than to pin down what's particularly good. ~ Leighton

* **Test User 3:**  Oh, meteor react. you poor bastards! That stuff is a pain in the ass to get the layout how you want. esp if you want it to autosize to window sizes. landing looks good, better than what my group did in that class. Someone on your team has design talent. If you want to users to be able to add pictures I can point you in the right direction. Also, I'd remove the Hours table from the Map page. It's redundant and takes away from your custom static map. ~ Ken

* **Test User 4:**  Review section doesn't have any reviews for many of the trucks. Buttons dont do anythings. All backgrounds are the same; I would like to see variety based on the restaurant. Really good work on the map! ~ Leighton

* **Test User 5:**  I like the logo. ~ Adrien

* **Test User 6:**  Love the color scheme and organization. The map is very readable, and it's smart to have a separate hours page. I suggest changing the white tables to have a brighter background, and add hours to the individual pages for each place.  Please left justify text - it is stressful to read. Very pretty colors and layout. ~ Liz

### Future Improvements

The work of a software developer is almost never finished. We know that there is always room for improvement, and that is definitely the case for our website. Here are a few areas that we will look to improve upon in future versions on our Snackademic site:

* Making the map dynamic
* Allowing Vendors to input their location and hours
* Integrating the picture upload feature for all accounts
* Displaying the hours on each Restaurant and Food truck info page.
