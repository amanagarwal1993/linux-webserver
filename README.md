# Linux Server Details

**Note**: This VM was configured for an academic (okay, academic-*ish*) project, meant to be open for all who came across my repo to play around with. But this VM has long been destroyed (AWS costs money!) and the private key mentioned below was exclusively created for this VM (never give your private key to anyone).

##### What you'll need to log in using *ssh*

- IP: **52.39.251.44**
- Port: **2200**
- Username: **grader**
- Private key: [grader_key](grader_key)
- Passphrase: **123456**

##### URL of hosted web application
[catalog.nextaltitude.com](http://catalog.nextaltitude.com)

##### Python packages required to deploy the Flask application
- Flask
- Jinja2
- DateTime
- psycopg2
- requests
- SQLAlchemy
- urllib3
- virtualenv

##### Linux packages required
- Postgres
- Apache2
- MOD_WSGI

##### Summary of configurations
1. Created super user **grader**, and enforced key-based authentication
2. Make server secure by setting up firewall
3. Upgrade and install required packages
4. Set up Flask application in a package structure
5. Create Postgres database with a user named *catalog*
6. Prepopulate the database using a python script
7. Deploy Flask application using Apache

###### No third party tools except Amazon Lightsail were used for this project.
