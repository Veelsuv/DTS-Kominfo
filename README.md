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
How Pages are Displayed<br>
When displaying a page, Rails returns views via its controllers.<br>
![image](https://user-images.githubusercontent.com/49402463/131250292-2381afc4-0d05-49f6-8cb0-5253cd865d04.png)<br>
```rails generate controller home top``` command creates a controller file named <b>home_controller.rb</b> with a top method. A method within a controller is also known as an <b>action.</b><br>
![image](https://user-images.githubusercontent.com/49402463/131250359-48206f2d-21a2-43e9-8889-3ccd2c1feedf.png)<br>
<br>
<b>Understanding Action</br>
The role of an action in a controller is to find a view from the views folder, then return it to the browser. The action looks for a folder with the same name as the controller (Home), then finds a file with the same name as the action (top).<br>
![image](https://user-images.githubusercontent.com/49402463/131250403-2f65fc7c-53a7-4175-9191-9ef379251188.png)<br>
<b>Understanding Routes</b><br>
This completes the process for displaying a web page.<br>
![image](https://user-images.githubusercontent.com/49402463/131250440-2ae8a5ad-3edb-4eaa-96f6-c67687c0a055.png)<br>
<br>
<b>The Role of Routes</b><br>
While we return the view through the controller, the routing is the one responsible for connecting the browser to the controller. Make sure to understand that the process for displaying a page is in the following order: routes → controllers → views.<br>
![image](https://user-images.githubusercontent.com/49402463/131250484-99cb8b67-6ab0-439a-b655-0b4c9045be36.png)<br><br>
Routes can be described with <b>a routing table.</b> A route points to a specific action of a controller according to the URL requested. When a URL is entered in the browser, it calls for a matching action in the controller based on the URL.<br>
![image](https://user-images.githubusercontent.com/49402463/131250529-f9d85ecb-83fd-4862-a936-4ad5a02630e3.png)<br><br>
<b>The Routes File</b><br>
Routes are defined in the config/routes.rb file in the following syntax: get "URL" => "controller#action". For instance, as shown in the image below, the URL "localhost:3000/home/top" points to the top action in the Home controller.<br>
![image](https://user-images.githubusercontent.com/49402463/131250572-a9274557-e732-45e9-a54f-77fa6c8fbb93.png)<br><br>
<b>Routing Errors</b><br>
you can't access a URL that isn't written in the routes file.<br>
![image](https://user-images.githubusercontent.com/49402463/131250665-cc75a14d-790b-4387-8d17-7104e28c30bf.png)<br><br>
<b>Changing a Route</b><br>
You can change the URL of the Top page by editing its route. Once you modify the route, you can access the Top page via localhost:3000/top. Even when the URL is changed, the view file (top.html.erb) is still displayed in the browser as long as the home#top remains the same.</br>
![image](https://user-images.githubusercontent.com/49402463/131250727-2487528e-e870-4958-8371-5b13cd576d3c.png)<br><br>
![image](https://user-images.githubusercontent.com/49402463/131250735-73bb1ebf-ae38-4c9d-adfa-4cf816b326d3.png)<br><br>



