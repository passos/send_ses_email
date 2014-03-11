send_ses_email
==============

A CLI script to send email via AWS SES

## Sample config file
Here is a sample config file

    [ses]                                                                           
    region=<YOUR AWS SES REGION>                                                    
    aws_access_key_id=<YOUR AWS SES ACCESS KEY ID>                                  
    aws_secret_access_key=<YOUR AWS SES SECRET KEY>


## Usage

    send_ses_email -c aws_config -t me@email.com -f no-reply@email.com -s "Hello, SES" -m 'Test Email'

    cat email_message.html | send_ses_email -c aws_config -t me@email.com -f no-reply@email.com -s "Hello, SES"


## Dependency
This script use AWS Python SDK to send email via SES. You can install the
dependency library by this command

    pip install -r requirements.txt


## License
This project is published under Apache License V2

