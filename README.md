# Monitoring-Book-API-with-Prometheus-and-Grafana
This project demonstrates the setup of a Book API with monitoring using Prometheus and visualization with Grafana. It involves deploying a RESTful service, configuring Prometheus to scrape metrics, and visualizing the data with Grafana, along with setting up alerting rules for tracking request rates.

**Overview**

This project implements a Book API, which exposes metrics for Prometheus to scrape and monitor various HTTP request metrics, such as the total number of requests per method (GET, POST, PUT,DELETE). These metrics are visualized using Grafana, which also allows the creation of alert rules to notify when specific thresholds are breached (e.g., too many requests per second).The architecture leverages Docker Compose for managing the services, Prometheus for collecting metrics, and Grafana for visualizing the data.

**Technologies Used**

This project utilizes a modern and containerized technology stack to ensure efficient development, monitoring, and deployment:

     ** Application**: Built using Node.js, the RESTful Book API provides core functionality and exposes metrics for monitoring.
      
      **Monitoring**: Prometheus is used to scrape and store real-time metrics from the Book API, enabling performance tracking and analysis.
      
      **Visualization**: Grafana offers a powerful interface to visualize metrics data from Prometheus and set up alerting rules for system observability.
      
      **Deployment**: Docker Compose orchestrates the multi-container setup, allowing seamless deployment and environment replication.
      
      **Database**: MongoDB (Cloud) is used as the primary NoSQL database to store and manage book records efficiently.


**Project Structure**


![image](https://github.com/user-attachments/assets/6857f94b-15a7-4846-a646-7dbd53cdcf32)




**Setup Instructions**
Build and Start the Containers
1. Clone the project repository to your local machine.
2. Navigate to the project folder:
      Go to the root of the project directory in your terminal.
3.  Build and start the containers:
      Use the following command to build and start the Docker containers:
        docker-compose up --build
This will build the Docker images and start the containers for the Book API, Prometheus, and Grafana.

4. Access the Services
    Once the containers are up and running, you can access the following services locally:
   
      Book API: http://localhost:3000/books    
      Prometheus: http://localhost:9090    
      Grafana: http://localhost:3001



**Conclusion**

This project demonstrates the full cycle of monitoring and visualization of a REST API using Prometheus and Grafana. By following the instructions, we were abled to:

        Set up a Book API with Prometheus metric exposure.        
        Configure Prometheus to scrape metrics from the API.        
        Deploy a Grafana dashboard to visualize the metrics.  
  
  Set up alerting in Grafana based on request rate thresholds.
This is a complete implementation of monitoring and alerting for a web service using Docker, Prometheus, and Grafana.
