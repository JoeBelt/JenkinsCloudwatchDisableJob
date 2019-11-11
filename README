Suppose you have a group of AWS events that you’d like to disable all at once. Such as when doing a deployment or scheduling system downtime, you might want an easy way for an admin to disable CloudWatch events without having to go through each event. One way is to utilize a Jenkins pipeline along with the aws cli to handle the disabling for you.

If you are running Jenkins on an EC2 instance, you can use the following code as a disabler. It gets the caller identity for the IAM role under which Jenkins is running and then gets all the CloudWatch event rules that start with the name “prod-events-” running in the region us-east-1.

To use this for your own environment, be sure to update “prod-events-” to the prefix for your events and set “us-east-1” to your region.
You’ll need the following Jenkins plugin installed for this to work.
Pipeline Utility Steps
