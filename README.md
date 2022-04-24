# Steps to start:
1. Run FirstApp and SecondApp applications
2. Run ./docker/docker-up.bat (after that Prometheus is available on http://localhost:9090, Grafana is available on http://localhost:3000)
3. To check if Prometheus is connected to apps, you need to go to http://localhost:9090/targets
4. Go to http://localhost:3000 and login with default username and password 'admin'
5. Change password
6. Click on the Datasource option under Configuration in the sidebar to add Prometheus as Datasource
7. Enter the HTTP url of Prometheus (http://EXTERNAL_IP:9090)
8. Click Save & Test
9. Click on the Import option under Create in the sidebar to import dashboard provided by Micrometer 
10. Choose the Micrometer JVM dashboard with id = 4701 and Prometheus Datasource
11. Click Import

Everything is running.