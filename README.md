# Planning my application
	1. Answer Questions
		- What am I building?
		- Who am I building it for?
		- What are the languages and/or frameworks am I going to use?
		- What features do I need to have?
	2. User Stories
	3. Model the Data
	4. Think through the pages I need in my app
   	5. 3rd party gems/packages I need to use in my app

## Questions

	1. I am building a personal/portfolio site. A place where I cab share examples of my work, and have people contact me.

	2. I am building it for myself. Show potential employers that what I know with real examples.

   	3.
		- Ruby on Rails
			- Ruby version 2.2.3p173
			- Rails version 4.2.6
		- HTML 5 or HAML
		- SCSS
		- jQuery
		- Materialize (see more in http://materializecss.com/)
		- Font Awesome (see more in https://fortawesome.github.io/Font-Awesome/)

	4.
		- Projects
			- Create / Edit / Destroy
		- Skills
			- Create / Edit / Destroy
		- Contact
			- Contact form (Sendgrid)
		- User (Devise)


## User Stories

	As a blank, I want to be able to blank, so that blank.
		- As a user, I want to be able to edit & destroy posts (of projects and skills), so that I can manage my portfolio.
		- As a user, I want to show the visitors and potential employers what are my main skills.
		- As a user, I want to show the visitors and potential employers examples of my work, or stuff I've built.
		- As a user, I want to be able to have visitors contact me through a form on my site.

## Model the Data

   	--Category--
      		name:string

	--Project--
		title:string
		category:Category
		update_date:date
		creators:text
		description:text
		languages:text
		github_link:string
		online_link:string (can be null)
		cover_image:string
		image:string

   	--Skill--
		language:string
		percent:integer

	--User--

## The pages I need in my app

	- Home
	- Projects#Index
	- Projects#Show
	- Skills#Index
	- About
	- Contacts

## 3rd party gems/packages

   - devise
   - mail_form
   - materialize-sass
