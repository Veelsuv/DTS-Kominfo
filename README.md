# DTS-Kominfo
# RUBY

<b>RUBY ON RAILS</b><br>
What's Ruby On Rails?<br>
Ruby on Rails is a framework used for developing web applications. 
With frameworks, you can significantly reduce the amount of work necessary for developing apps.

<b>Generating a Rails Application</b><br>
You first need to prepare some folders and files.
This can be generated using the rails command.

```$ rails new application_name```<br>
ex : ```$rails new tweet_app```
![image](https://user-images.githubusercontent.com/49402463/131249755-d0d66b68-0a49-4f24-949a-50d7e11eb0c0.png)
<br>
<b>Starting Server</b><br>
To see the application in the browser, you need to start the server with the ```rails server``` command. After running this command, you'll see the default page when you access the URL ```localhost:3000``` in the browser.<br>
<b>Creating Top Page</b><br>
You can create the Top page with the ```rails generate controller home top``` command. A new web page is automatically created by this command, and will allow you to access ```localhost:3000/home/top```.<br>

![image](https://user-images.githubusercontent.com/49402463/131249969-5b9c51bf-7198-4d1a-bf51-b1a513802300.png)
<br>
<b>Understanding Views</b><br>
How can a page be generated just by a command?<br>
Well, when you run the command ```rails generate controller home top```, Rails generates all the necessary files for displaying a page.<br>
To display a page in Rails, you need the three things shown in the image on the below<br>
![image](https://user-images.githubusercontent.com/49402463/131250066-806d678d-596c-4895-8c73-0e42058589ea.png)
<br>
A view is an HTML file that's used to create the look of a page. When the browser asks Rails for a file, Rails returns a requested view to the browser to display a page.<br>
Views are located inside the views folder. The rails generate controller home top command generates the home folder and a file named top.html.erb in the views folder. erb is a unique file format, but you can think of it as a regular HTML file for now.<br>
![image](https://user-images.githubusercontent.com/49402463/131250125-0526a26d-5e11-43bd-abfc-f19e32aeef3c.png)<br>
![image](https://user-images.githubusercontent.com/49402463/131250134-51ccba03-1170-4ba8-9149-fee2d067aef9.png)<br>

<b>Understanding Controllers</b><br>
![image](https://user-images.githubusercontent.com/49402463/131250169-bea7ca45-f9ea-45e9-a946-72802b8a7a24.png)<br>
<u>How Pages are Displayed</u><br>





