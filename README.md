# Travel Memory

<ul>
<h1>Backend Configuration</h1>
  <li>Clone the repository and navigate to the backend directory</li>
  <li>The backend runs on port 3000. Set up a reverse proxy using nginx to ensure smooth deployment on EC2</li>
  <li>Update the .env file to incorporate database connection details and port information</li>
  ![EC2_instance](https://github.com/user-attachments/assets/00bb51f1-93d8-4e04-9636-c219bb3679dc)

<h1>Frontend and Backend Connection</h2>
    
  <li>Navigate to the `urls.js` in the frontend directory</li>
  <li>Update the file to ensure the front end communicates effectively with the backend</li>

<h1>Scaling the Application</h3>
  <li>Create multiple instances of both the frontend and backend servers</li>
  <li>Add these instances to a load balancer to ensure efficient distribution of incoming traffic</li>
<h1>Domain Setup with Cloudflare</h4>
  
  <li>Connect your custom domain to the application using Godady</li>
  <li>Add these instances to a load balancer to ensure efficient distribution of incoming traffic</li>
<h1>Documentation</h5>


  <li>Fourth item</li>
  <li>Fourth item</li>
  <li>Fourth item</li>
  <li>Fourth item</li>
  <li>Fourth item</li>
  <li>Fourth item</li>
  <li>Fourth item</li>
  <li>Fourth item</li>
  <li>Fourth item</li>
    
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
