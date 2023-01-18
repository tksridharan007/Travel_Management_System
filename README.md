# Travel_Management_System
A travel management system is a software product that manages all components of your business travel.  Typically they are integrated with travel service providers, offering real-time quotes, bookings, and trip logistics in one place.  Managers can track bookings, cancellations, adjustments, and rescheduling in real-time, eliminating a lot of the manual back and forth that previously had to happen through email.In today’s modern era where travel is such a crucial part of operations.

# Installation
# Prerequisites
# 1. Install Python
Install python-3.3.2 and python-pip. Follow the steps from the below reference document based on your Operating System. Reference: https://docs.python-guide.org/starting/installation/

# 2. Install MySQL
Install mysql-8.0.15. Follow the steps form the below reference document based on your Operating System. Reference: https://dev.mysql.com/doc/refman/5.5/en/

# 3. Setup virtual environment
          # Install virtual environment
              sudo pip install virtualenv
          # Make a directory
              mkdir envs
            
            # Create virtual environment
                   virtualenv ./envs/

            #Activate virtual environment
                  source envs/bin/activate


# 4. Install requirements

        1. asgiref==3.2.10
        2. Django==3.1.2
        3. mysql-connector-python==8.0.22
        4. mysqlclient==2.0.1
        5. protobuf==3.13.0
        6. pytz==2020.1
        7. six==1.15.0
        8. sqlparse==0.4.1

# 5. Create Database in MySQL
           
           create database Travel_Management_System(In MongoDB);

# 6. Edit project settings

           # open settings file
           # Edit Database configurations with your MySQL configurations.
           # Search for DATABASES section.
                DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'Travel_Management_System',
        'USER': '<mysql-user>',
        'PASSWORD': 'sridharan',
        'HOST': '<mysql-host>',
        'PORT': '<mysql-port>',
    }
}
# save the file

# 7. Run the server
          # Make migrations
              python manage.py runserver
                    Try opening http://127.0.0.1:8000/ in the browser. 

# 9. URLs

1. Login Page -- http://127.0.0.1:8000/loginmodule/login/
![image](https://user-images.githubusercontent.com/82249340/213260905-f5674da7-07a2-45ba-80b2-201ba7ef9b65.png)
2. Admin Page -- http://127.0.0.1:8000/admin/login/?next=/admin/
![image](https://user-images.githubusercontent.com/82249340/213261222-8199120c-8cc8-4b0a-968b-8da478fc5e3d.png)


