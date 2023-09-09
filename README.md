<div align="center">
  <h1>Building and Securing a Microservices E-commerce Application</h1>
</div>

<div>
  <h2>Saleor</h2>
</div>
<p>Saleor is an open-source e-commerce platform built using Django, GraphQL, and React. It is intended to give developers with a flexible and customizable foundation for building online storefronts and e-commerce apps. Saleor is available on GitHub, where you can contribute to its development.</p>

<div>
  <h2>How to Create a Kubernetes Cluster on GKE</h2>
</div>

<div>1.	Login into your Google Cloud Account.</div>
<div>2.	Create a new Project and name it as “ISEC6000”.</div>
<div>3.	In the ISEC6000 project, Click Kubernetes Engine  Cluster  Enable the Api  Create.</div>
<div>4.	Select and configure under the Standard cluster mode.</div>
<div>5.	Configure a cluster with the name isec6000-cluster-1-assignment1 and set the zone as us-central1-c under the zonal location type.</div>
<div>6.	Configure the default Kubernetes version and node pool with 3 nodes.</div>

<div>
  <h2>How to INSTALL AND CONFIGURE KUBERNETES</h2>
</div>

<div>1.	The Cluster isec6000-cluster-1 is created as shown in Fig 1.2.1</div>
<div>2.	Connect the Kubernetes Cluster to the local environment.</div>
<div>3.	Select Activate Cloud shell to open the shell terminal.</div>
<div>4.	Set the project with the project ID and configure the zone using the following commands:</div>
<div align="center">-gcloud config set project isec6000-397505</div>
<div align="center">-gcloud config set compute/zone us-central1-c</div>

<div>
  <h2>How to Create Git Repository</h2>
</div>

<div>1.	Create a new Repository and name it as “ISEC6000Assignment1Task1”.</div>
<div>2.	Set the Repository as public and select the checkbox with add a README file option.</div>
<div>3. A repository is created as shown in Fig 1.2.3</div>
<div>4.	The Repository can be accessed through the below link. </div>
      -https://github.com/Aravind1025/ISEC6000Assignment1Task1

<div>
  <h2>How to Fork Saelor Platform in Git Repository</h2>
</div>

<div>1.	Using the below link, fork the Saelor Platform from Git</div>    
     <div>-https://github.com/saleor/saleor-platform</div>
<div>2. Rename it as “saleor-platform-Assignment1Task2”.</div>
<div>3. New Repo can be accessed through the link</div>
      <div>-https://github.com/Aravind1025/saleor-platform-Assignment1Task2.git</div>

<div>
  <h2>How to ASSIGN THE CONTAINER PORTS</h2>
</div>

<div>1. Examine the functionalities of the Saleor platform and explore the ports in the docker-compose.yml file.</div>
<div>2. Assign the Saleor Store-front port to 3009 and the saleor dashboard ports to 9003.</div>
<div>3. Commit the changes in the Git Repository.</div>
<div>4. To clone the Git Repository:</div>
      <div>git clone https://github.com/Aravind1025/saleor-platform-Assignment1Task2.git</div>
<div>5. To go into the Repository:</div>
      <div>cd saleor-platform-Assignment1Task2</div>
<div>6. To Build the Repository:</div>
      <div>docker compose build</div>
<div>7. To Apply Django migration:</div>
      <div>docker compose run --rm api python3 manage.py migrate</div>
<div>8. To create the admin user and fill the database with sample admin data</div>
      <div>docker compose run --rm api python3 manage.py populatedb –createsuperuser</div>
<div>9. To execute the Application</div>
      <div>docker compose up</div>
<div>10. Once the containers are created, we can access the Saelor Store-front UI in our local environment.</div>
      <div>React-StoreFront accessible at https://localhost:3009</div>
      <div>Saleor Dashboard accessible at https://localhost:9003</div>

<div>
  <h2>TRIVY</h2>
</div>

<div>Trivy is an open-source vulnerability scanner. It is reliable, fast and extremely easy to use. Trivy has different scanners that look for different security issues, and different targets where it can find those issues.</div>

<div>
  <h2>Steps to Install Trivy</h2>
</div>

<div>1.	wget https://github.com/aquasecurity/trivy/releases/download/v0.20.0/trivy_0.20.0_Linux-64bit.tar.gz</div>
<div>2.	tar zxvf trivy_0.20.0_Linux-64bit.tar.gz</div>
<div>3. sudo mv trivy /usr/local/bin/</div>

<div>
  <h2>To Scan the Vulnerability of TRIVY</h2>
</div>
Syntax: trivy image {image Name} 








