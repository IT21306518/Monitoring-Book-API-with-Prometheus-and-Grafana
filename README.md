# Monitoring-Book-API-with-Prometheus-and-Grafana
This project demonstrates the setup of a Book API with monitoring using Prometheus and visualization with Grafana. It involves deploying a RESTful service, configuring Prometheus to scrape metrics, and visualizing the data with Grafana, along with setting up alerting rules for tracking request rates.

**Overview**

This project implements a Book API, which exposes metrics for Prometheus to scrape and monitor various HTTP request metrics, such as the total number of requests per method (GET, POST, PUT,DELETE). These metrics are visualized using Grafana, which also allows the creation of alert rules to notify when specific thresholds are breached (e.g., too many requests per second).

The architecture leverages Docker Compose for managing the services, Prometheus for collecting metrics, and Grafana for visualizing the data.

**Technologies Used**


![image](https://github.com/user-attachments/assets/6d6d9019-610c-4c74-92c9-087271b6e6a2)


**Project Structure**


![image](https://github.com/user-attachments/assets/8055238f-b16c-4665-9130-f908a3b0301b)


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
