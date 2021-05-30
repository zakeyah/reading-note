# AWS: S3 and Lambda

 ### Amazon Simple Storage Service (Amazon S3)
 #####  is an object storage service that offers industry-leading scalability, data availability, security, and performance. This means customers of all sizes and industries can use it to store and protect any amount of data for a range of use cases.

 ### AWS Lambda Basics
 #### AWS Lambda is a service which computes the code without any server. Code is executed based on the response of events in services such as adding/removing files in S3 bucket. 

#### The Lambda functions can perform any kind of computing task, from serving web pages and processing streams of data to calling APIs and integrating with other AWS services

#### Each Lambda function runs in its own container
#### When a function is created, Lambda packages it into a new container and then executes that container on a multi-tenant cluster of machines managed by AWS
#### Before the functions start running, each function’s container is allocated its necessary RAM and CPU capacity
#### Once the functions finish running, the RAM allocated at the beginning is multiplied by the amount of time the function spent running


### CDN
#### Content Delivery Network
![](https://psycray.com/wp-content/uploads/2020/10/image11.jpg)


####  is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.