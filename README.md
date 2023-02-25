# Teacher-Portal
## Project Overview
### Task Description:
The task is to create a teacher's portal that is handled using local storage. The portal consists of three HTML pages - index, login, and dashboard.html. Here are the tasks to be accomplished:

As soon as the teacher goes to the index page, they will be asked to sign up. Basic email and password validations will be done, such as ensuring that the password and confirm password match, email should be a valid email format, the name should not be empty, etc.

Once the teacher clicks on signup, an array of users will be created, and the teacher's user with all their details will be appended to that array. This array will be stored in the local storage. The local storage should look like this -
users = [{email:teacher1@gmail,pass:123232,name:"Teacher 1 Name"},{email:teacher2@gmail.com,pass:!23454,name:"Teacher2 Name"}]

After signup, the teacher will be taken to the login page where they can log in using their credentials. If the teacher's object exists in the users array stored in the local storage, they will be logged in. A new local storage item will be created called currentUser, which will look like this -
{email:teacher1@gmail,pass:123232,name:"Teacher 1 Name",token:"shgvyiqwuyfq67221"} where the token is a randomly generated 16 character string.

Once the login is successful, the teacher will be taken to the dashboard page where they can change their password, but only if the old password matches. There will also be a logout button, which when clicked, will remove the currentUser state and make it null.

Basic validations will be implemented everywhere, and if the current user exists, they will be taken directly to the dashboard.html page instead of the login or the index.html page. The users localStorage item is an array so that multiple users can sign up and log in. This must also be handled.

![image](https://user-images.githubusercontent.com/74090703/221373042-08b6c590-fe53-4a8e-ae36-f4096767da3d.png)
![image](https://user-images.githubusercontent.com/74090703/221373080-57db9c15-d556-4193-8faa-2cca8eb3185f.png)
![image](https://user-images.githubusercontent.com/74090703/221373106-e789e3d1-9a82-45ef-a04b-97d684126b7c.png)

