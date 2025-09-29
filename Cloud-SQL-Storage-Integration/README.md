# Cloud SQL + Cloud Storage Integration

##  Objective

Set up a *web server with PHP* on a Compute Engine instance, configure it to connect to a *Cloud SQL database*, and reference an image hosted in a *Cloud Storage bucket*.

---

##  Tools & Services Used

1. Compute Engine (VM instance – "bloghost")
2. Cloud Storage (bucket + object)
3. Cloud SQL (MySQL database)
4. PHP + Apache Web Server

---

##  Steps Performed

1. Created a Compute Engine VM ("bloghost") with Apache, PHP, and MySQL libraries installed.
2. Deployed a Cloud Storage bucket and uploaded a public image.
3. Created a *Cloud SQL instance (MySQL)* with user credentials and authorized VM access.
4. Edited the VM’s "index.php" file to connect to the Cloud SQL instance using the database IP and credentials.
5. Verified database connectivity via the PHP web app.
6. Modified "index.php" to reference the Cloud Storage image, displaying it on the web page.

---

##  Key Learnings

1. Compute Engine VMs can host web apps that integrate with *Cloud SQL** databases.
2. Cloud Storage provides a simple way to host static assets like images.
3. Application connectivity requires correct *firewall rules** and *authorized networks*.
4. Separating app, database, and storage layers improves scalability and reliability.

---

##  Real-World Application

This pattern mirrors a common **3-tier architecture**:

1. *Frontend/Web Tier* → VM with web server
2. *Database Tier* → Cloud SQL
3. *Storage Tier* → Cloud Storage

It’s a foundation for hosting blogs, CMSs (like WordPress), or small business apps in the cloud.

---

##  Reflection

This lab tied together multiple Google Cloud services into one application. I learned how networking and permissions connect app, database, and storage layers. It clarified how cloud apps scale by decoupling components.
