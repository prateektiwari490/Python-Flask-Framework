creating virtual env -->> py -3 -m venv venv
for activating virtual env -->> venv\Scripts\activate
for downloading boilerplate -->> http://www.initializr.com/

for 8 byte encrypted key
import os
os.urandom(8)

installing WTform is a library provide lot of features of form
pip install flask-wtf

downloading database for flask
pip install flask-sqlalchemy

Bcrypt
pip install flask-bcrypt

pip install flask-bcrypt

# see how it works


python

from flask_bcrypt import Bcrypt
bcrypt = Bcrypt()

# hash a password

bcrypt.generate_password_hash('testing')

# it generates a password 
# to decode it
# to get regular string

bcrypt.generate_password_hash('testing').decode('utf-8')

# each time we get a different hash

# save this hash password as a variable

hashed_pw = bcrypt.generate_password_hash('testing').decode('utf-8')

bcrypt.check_password_hash(hashed_pw, 'password')
# we get False values

bcrypt.check_password_hash(hashed_pw, 'testing')


after inserting some data

>>> from flask_package import db
>>> from flask_package.models import User
>>> user = User.query.first()
>>> user
	User('prateek','prateek@gmail.com', 'default.jpg')
>>> user.password
	b'$2b$12$i.y3CLD20NKMktvAw9EFO.jmGpduOr2NpoyxvdCjT1RsWmru49N4W'
>>> exit()


pip install flask-login



lets say i develop brand new gui for 
end user to key in input data and then 
when it tries to invoke any REST API then 
prior to that we need authorization so there 
certificates are required to authorize user.
that cert i was referring to

https://hubconnect.uhg.com/thread/138342