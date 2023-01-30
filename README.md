# Lambda_Creation_demo
Basic code for an AWS Lambda

Copied from A Cloud Guru, Cloud Practitioner course

def lambda_handler(event, context):
    message = 'Hello {} {}! Keep being awesome!'.format(event['first_name'], event['last_name'])  

    #print to CloudWatch logs
    print(message)

    return { 
        'message' : message
    }   
