# Astronomy Club Website

## Mentors
- Ansh Puvvada
- Nishant Sachdeva
- KV Aditya

## New Contributors:
1. Clone the repo on your local machine
2. Install hugo (v0.59 and above).
3. Find issues with the club website
4. Provide ideas and suggestions for improvement
5. Contribute by providing content or help in designing the pages 

# Club Website Creation 

The website is built with Hugo. 

## Updating Content or Design

1. Go to the `content` folder to update content like event content
2. Go to `layouts` folder to update the webpage design
2. GO to `data` to update events,images, site params,etc 
5. `team.yml` contains the memebers of the club, modify it accordingly.
6. `activities.yml` contains the list of major events the club does and gets listed in the homepage of your club. 
7. `event.yml` shows a list of events conducted and gets displayed as a gallery, on the events page. 
5. Modify the `title` and `type` in `event.yml` to reflect the events in `activities.yml`.

## Deploying the site on the local machine 
1. We use, `Hugo` a static site generater to generate the website. 
2. Install [Hugo](https://gohugo.io/getting-started/installing/) 
5. Run `hugo server` to run the server on your local machine. Execute this command in the root directory of the project. 
6. If you have drafts, then run `hugo server -D` to view them. Do not keep drafts, and set the value to `False` when you're done as they do not get deployed on the site.  
7. Make sure to have the latest version Hugo installed. 

## Adding Content 

1. Run `hugo new event_name.md` in the `/content/your-club-name/archive`. 
2. All the content posts are written in Markdown, and you can look into the Hugo Documentation for more details.
3. Modify the `event.yl` file in the `/data/your-club-name/`, and add a picture for that event. 
4. Make a new entry directly below the old ones, and give it a picture, and link it to the event-post created in the archive section done earlier. You can do a hardlink if you want(site is deployed on www.clubs.iiit.ac.in/clubs/your-club-name), but preferably make it a relative link, with the link being `{{< ref "/your-club-name/archive/my-post" >}}`.
5. Add the relavant `type` for it. 
6. If you want to add more than one picture make a seperate entry in `activities,yml


## Modifying homepage 

1. Go to `layouts/your_club/index.html` and modify the files over there 
2. Go to `data\your_club\homepage.yml` and modify the Hugo variables from there. 
3. Make sure to go to `layouts/partials/club_name/header.html` and change the home path to your club name from `club_name`
The names and the rest are pretty self-explanatory. In case you don't like it, you are free to rewrite `index.html` however you like as a normal html file. 
6. Make sure to have the latest version Hugo installed. I'm currently running v0.59.1. 

## Adding events to your club 

1. Take a look at data. 

## Issues or Doubts

Raise a GitHub issue, and I'll get back to you within a day. 