# VungLiemTown Documentation

## 1. Project Idea

### Overview
VungLiemTown is an online community platform designed for the residents of Vũng Liêm. The platform aims to provide various functionalities that enhance entertainment, social interaction, and local commerce. The primary focus is on creating a user-friendly experience that prioritizes entertainment while also offering essential services to the community.

### Core Features
- **Video Player & Fun Images**: Users can view and upload entertaining videos and images.
- **Online Karaoke**: A karaoke feature for users to sing along with their favorite songs.
- **Facebook Data Crawling**: Crawl data from local Facebook groups to create news and statistics, attributing posts to their original authors.
- **Online Marketplace**: A platform for users to upload and sell their products.
- **Online Store**: A feature for local business owners to manage their products and sales.
- **Food Delivery**: Users can order food online from local restaurants.
- **Ride-Hailing Service**: A service for drivers to accept bookings when they are available.
- **Business Directory**: A categorized directory of local businesses and shops.
- **Clubs & Groups**: A feature for users to join clubs and groups with similar interests.
- **Weather Forecast & Local News**: Provide weather updates, power outage schedules, and local news.
- **Job Portal**: A platform for job seekers and employers in Vũng Liêm.
- **Charity Section**: A section dedicated to helping those in need.
- **Business Advertising**: Paid advertising options for businesses.
- **Mini Games**: Fun games to entertain users during their free time.

### Prioritization
The primary criterion for the platform is entertainment, ensuring that users have a fun and engaging experience.

---

## 2. Directory Structure

### Project Directory Structure


### Project Directory Structure

```plaintext
VungLiemTown/
│
├── auth-service/
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── utils/
│   │   ├── index.js
│   │   └── config.js
│   ├── tests/
│   └── Dockerfile
│
├── user-service/
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── utils/
│   │   ├── index.js
│   │   └── config.js
│   ├── tests/
│   └── Dockerfile
│
├── product-service/
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── utils/
│   │   ├── index.js
│   │   └── config.js
│   ├── tests/
│   └── Dockerfile
│
├── api-gateway/
│   ├── src/
│   │   ├── routes/
│   │   ├── middleware/
│   │   ├── index.js
│   │   └── config.js
│   ├── tests/
│   └── Dockerfile
│
├── crawler/
│   ├── src/
│   │   ├── scripts/
│   │   ├── utils/
│   │   ├── index.py
│   │   └── config.py
│   ├── tests/
│   └── Dockerfile
│
├── web-app/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── utils/
│   │   ├── App.js
│   │   └── index.js
│   ├── tests/
│   └── Dockerfile
│
├── mobile-app/
│   ├── android/
│   ├── ios/
│   ├── src/
│   │   ├── components/
│   │   ├── screens/
│   │   ├── services/
│   │   ├── utils/
│   │   ├── App.js
│   │   └── index.js
│   ├── tests/
│   └── Dockerfile
│
├── docker-compose.yml
├── README.md
└── .gitignore
```



---

## 3. System Infrastructure

### Overview
The system infrastructure for VungLiemTown is designed to support a microservices architecture, allowing for scalability, maintainability, and independent deployment of services. The infrastructure will utilize Docker for containerization and Docker Compose for orchestration.

### Components
1. **Microservices**: Each core functionality (authentication, user management, product management, etc.) is encapsulated in its own microservice.
2. **API Gateway**: Acts as a single entry point for all client requests, routing them to the appropriate microservice.
3. **Crawler**: A dedicated service for crawling data from Facebook and other sources to populate the platform with relevant content.
4. **Web Application**: A React-based web application for users to interact with the platform.
5. **Mobile Application**: A React Native-based mobile application for users to access the platform on their mobile devices.
6. **Database**: PostgreSQL will be used for data storage, with optimizations for search functionality.
7. **Storage**: Files (images, videos) will be stored on a cloud service like AWS S3 or OpenDrive.
8. **Load Balancer**: To distribute incoming traffic across multiple instances of services for better performance and reliability.

### Deployment
- **Docker**: Each service will be containerized using Docker, allowing for consistent environments across development, testing, and production.
- **Docker Compose**: Used to define and run multi-container Docker applications, making it easy to start all services with a single command.
- **Cloud Hosting**: The application can be hosted on cloud platforms like AWS, Google Cloud, or DigitalOcean for scalability and reliability.

---

### Conclusion
VungLiemTown aims to create a vibrant online community for the residents of Vũng Liêm, providing entertainment and essential services. The microservices architecture will ensure that the platform is scalable and maintainable, allowing for future growth and feature enhancements.
