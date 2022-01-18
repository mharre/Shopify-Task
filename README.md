# Shopify-Task
INSTRUCTIONS ON HOW TO RUN
1) Copy repository 
2) Make sure python is installed
3) Create virtual env if wanted with the command(in terminal):
  python -m venv .venv 
4) Open copied repo, I personally use VScode so I just navigate to my folder in the directory and type: code .
5) If venv was created activate it with:
  source .venv/scripts/activate (please note you may have to cd into a different folder where the venv was created - something like source e_com/.venv.....)
6) In terminal type:
  pip install -r requirements.txt
7) In terminal:
  python manage.py makemigrations
  python manage.py migrate
8) Most likely will have to create a superuser, in the terminal please type the following command:
  python manage.py createsuperuser
    - this will prompt you with information on the user, I would suggest keeping it simple
    - username: admin
    - email: admin@admin.com
    - password: admin
    - y (type y then hit enter because it will tell you that the password is too simple but you can continue either way)
9) In terminal:
 python manage.py runserver
10) Visit localhost: localhost:8000/ to see the homepage
11) Type in localhost:8000/admin and login with the credentials that you created above which will bring you to the admin page
12) On the menu in the left hand side select artist, the plus symbol and type a random name and click save in the bottom left of the page
13) Select product from the menu in the left hand side, in the top left click add product
14) Fill out the information any way you like, you can leave discount price blank but all other fields must be filled
15) Upload the image provided in inventory_example, you can upload as many as you want but the website is scalable so it works the same way for 1 image or many
16) Navigate back to home page (localhost:8000)
17) The image should appear at the bottom of the page, or click on your cart on the top right to be redirected to the inventory
18) Select the product, more information, and then add the item to your cart
19) Click on your cart, then click proceed to checkout (change the quantity if you want to test adding more than 1)
20) Fill out the fields with random information, check billing address is the same as shipping to speed up this process, then check stripe, and click continue to checkout
21) Type 4242424242424242 for everything in the field (this is stripes test payment) and click submit payment (upon success a message should pop up and a redirect)
22) Visit localhost:8000/admin again
23) You can now view Orders from the left menu which keeps track of all orders and the account that ordered them
24) You can now request a refund from the profile section, or change shipping status, refund status etc from admin panel as well
25) This was the first website which I ever created and it was made completely from scratch
26) Thank you!
