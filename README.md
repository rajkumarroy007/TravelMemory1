# Travel Memory

<ul>
<h1>Backend Configuration</h1>
  <li>Clone the repository and navigate to the backend directory</li>
  <li>The backend runs on port 3000. Set up a reverse proxy using nginx to ensure smooth deployment on EC2</li>
  <li>Update the .env file to incorporate database connection details and port information</li>
  
![EC2_instance](https://github.com/user-attachments/assets/00bb51f1-93d8-4e04-9636-c219bb3679dc)
![backend2](https://github.com/user-attachments/assets/ad1534c3-1165-42fd-afbf-2c8f787cf526)
<h1>Frontend and Backend Connection</h2>
    
  <li>Navigate to the `urls.js` in the frontend directory</li>
  <li>Update the file to ensure the front end communicates effectively with the backend</li>

![Frontend](https://github.com/user-attachments/assets/19b27a3f-1f84-4bfc-aede-2ed183aa1082)
![Frontend2](https://github.com/user-attachments/assets/4c4de929-1481-4437-b4f5-e7a8d42ded2c)

<h1>Scaling the Application</h3>
  <li>Create multiple instances of both the frontend and backend servers</li>
  <li>Add these instances to a load balancer to ensure efficient distribution of incoming traffic</li>
  
![LB](https://github.com/user-attachments/assets/c74c4d31-edbf-4633-a54b-a99004029990)
  
<h1>Domain Setup with Cloudflare</h4>
  
  <li>Connect your custom domain to the application using Godady</li>
  <li>Add these instances to a load balancer to ensure efficient distribution of incoming traffic</li>

![CNAME](https://github.com/user-attachments/assets/6c483b83-1799-4934-bfff-c478edd52af0)

![Godady Cname record](https://github.com/user-attachments/assets/88489055-82f4-4f57-9b3f-953ba66d53bc)
  
<h1>Documentation</h5>


    
</ul>


`.env` file to work with the backend after creating a database in mongodb: 

```
MONGO_URI='ENTER_YOUR_URL'
PORT=3001
```

Data format to be added: 

```json
{
    "tripName": "Incredible India",
    "startDateOfJourney": "19-03-2022",
    "endDateOfJourney": "27-03-2022",
    "nameOfHotels":"Hotel Namaste, Backpackers Club",
    "placesVisited":"Delhi, Kolkata, Chennai, Mumbai",
    "totalCost": 800000,
    "tripType": "leisure",
    "experience": "Lorem Ipsum, Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum, ",
    "image": "https://t3.ftcdn.net/jpg/03/04/85/26/360_F_304852693_nSOn9KvUgafgvZ6wM0CNaULYUa7xXBkA.jpg",
    "shortDescription":"India is a wonderful country with rich culture and good people.",
    "featured": true
}
```
