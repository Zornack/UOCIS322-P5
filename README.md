# UOCIS322 - Project 5 #
Author: Jaryd Davis, jcsdavis@gmail.com

An ACP brevet time calculator.

Dockerfile included for ease of use with docker build and docker run.

Distances input as miles are converted to kilometers then floored. Distances input as kilometers are rounded to the nearest digit.

Kilometer distances are converted to opening and closing times following the minimum and maximum speeds listed here: https://rusa.org/pages/acp-brevet-control-times-calculator

Opening and closing times are added to the user entered starting time.

Negative distances return null values and an error message. Distances 20% longer than the brevet distance include an error message.

acp_times calculates the opening and closing times and returns an arrow object

flask_brevets pulls km, brevet distance and starting time from the client, then returns the opening and closing times.

javascript updates the page asynchonrasly via AJAX and jQuery.

Test calculations included for debugging. Run with nosetests. Edit tests/test_brev.py for further testing.

Insert adds km, open and close times to a database. Requires a valid final control. Inserting clears the last inserted values from the database.

Display renders a new page with the data from the database.


## Credits

Michal Young, Ram Durairajan, Steven Walton, Joe Istas.