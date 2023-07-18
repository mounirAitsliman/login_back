# login_back
run the following queries to populate your role table

INSERT INTO roles(name) VALUES('ROLE_USER'); </br>
INSERT INTO roles(name) VALUES('ROLE_MODERATOR'); </br>
INSERT INTO roles(name) VALUES('ROLE_ADMIN'); </br>

testing the api/v1/auth/signup endpoint
![img.png](Readme_images/img.png)

testing the api/v1/auth/signin endpoint
![img_1.png](Readme_images/img_1.png)

testing public api/v1/test/all 
![img_2.png](Readme_images/img_2.png)

testing (must be authentificated regardless of the role that you have) api/v1/test/user

![img_3.png](Readme_images/img_3.png)

testing the same last endpoint but this time we passed the jwt in the header 

![img_4.png](Readme_images/img_4.png)

testing the endpoint of the moderator /api/v1/test/mod (the principal "currently logged in user" has the mod authorization)

![img_5.png](Readme_images/img_5.png)

trying to access the endpoint of the admin with mod permission (api/v1/test/admin)

![img_6.png](Readme_images/img_6.png)

