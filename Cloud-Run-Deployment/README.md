# Hello Cloud Run – Deploying a Containerized Application

##  Objective

Build, containerize, and deploy a simple *Node.js application** using *Cloud Run*, Google Cloud’s fully managed serverless platform.

---

##  Tools & Services Used

1. Cloud Run
2. Cloud Build
3. Artifact Registry
4. Docker
5. Node.js / Express

---

##  Steps Performed

1. Enabled the *Cloud Run API* and set up environment in Cloud Shell.
2. Wrote a simple Node.js Express app ("index.js` with "Hello World" route).
3. Created a "Dockerfile" and containerized the app.
4. Built and pushed the image to *Artifact Registry* with Cloud Build.
5. Deployed the container to *Cloud Run* with "gcloud run deploy".
6. Verified deployment via the public service URL.
7. Cleaned up resources (removed image and Cloud Run service).

---

##  Key Learnings

1. *Cloud Run abstracts infrastructure management*, allowing focus on app code.
2. Deploying containers is streamlined with Cloud Build + Artifact Registry.
3. Cloud Run scales automatically to handle requests, then scales down when idle.

---

##  Real-World Application

This is directly applicable to *modern DevOps workflows*—build a container, deploy to Cloud Run, and let Google handle scaling, networking, and infrastructure. Perfect for *APIs, microservices, and lightweight apps*.

---

##  Reflection

This lab was a solid introduction to *serverless container deployment*. I gained hands-on experience with containerization, registry management, and deployment. Next, I’d like to explore connecting Cloud Run services to databases or private VPCs.
