# my-static-website Project
In this mini project, I will establish a static website using Amazon S3's static website hosting feature. This project will guide me through the process of creating an S3 bucket, uploading static website content, configuring the bucket for static website hosting, and testing the hosted website.

### Objectives:

1. Create an S3 Bucket
1. Upload Static Website Content
1. Configure the S3 Bucket for Static Website Hosting
1. Test the Hosted Website

### Tools Utilized for This Project Include:
1. Git: Throughout the project, Git was used to create repositories, commit changes, branch, merge, and keep a history of the codebase development. This facilitated effective version control and enabled collaboration.

1. GitHub: The project repository was hosted on GitHub, allowing for centralized storage and easy access to the code. GitHub also provided features for issue tracking, pull requests, and collaboration with other developers.

3. Visual Studio Code: Visual Studio Code was used for writing, editing, and debugging the HTML, CSS, and JavaScript files that make up the static website. Its integration with Git allowed for seamless version control operations directly from the editor.
4. Markdown: Markdown was used to create detailed documentation for the project. This included writing README files, documenting the steps followed, the configuration details, observations, challenges, and insights gained during the project.

These tools collectively facilitated efficient development, version control, documentation, and collaboration, ensuring the smooth completion of the static website hosting project on Amazon S3.

### Comprehensive Steps and Documentation
The following screenshots show the comprehensive steps I took to arrive at the goal of my project, as well as issues identified and solutions implemented:

### Task 1: Create an S3 Bucket
- On the Amazon S3 dashboard, click the "Create bucket" button. Enter a unique name for my bucket.
![](./img/task%201/1.bucket-name.png)

- Choose the appropriate region for my bucket.
![](./img/task%201/2.bucket-region.png)

- Uncheck "Block all public access" to allow public access (I'll need this for static website hosting).
![](./img/task%201/3.Uncheck-Block-all-public-access.png)

- Click "Create bucket" to finalize the creation.
![](./img/task%201/4.bucket-CREATE-BUTTON.png)
![](./img/task%201/5.bucket-created.png)

### Task 2: Upload Static Website Content

- Ensure you have all the necessary files (e.g., index.html, styles.css, images, etc.) ready for upload.
![](./img/task%202/1.static-website-files-gathered.png)
![](./img/task%202/2.file-structure.png)

- In the Amazon S3 dashboard, I will navigate to my newly created bucket and Click the "Upload" button and follow the prompts to upload my static website files.
![](./img/task%202/3.click-on-upload.png)
![](./img/task%202/4.uploaded.png)

### Task 3: Configure S3 for Static Web Hosting
- Go to the "Properties" tab of my S3 bucket.
![](./img/task%203/1.Go-to-Properties.png)

- Scroll down to the "Static website hosting" section.
![](./img/task%203/2.Scroll-to-Static-website-hosting-CLICK-EDIT.png)

- Select "Enable" under "Static website hosting." Set the "Index document" to index.html.
![](./img/task%203/3.enable-and-index.png)

- Save the changes.
![](./img/task%203/4.Save-changes.png)

### Task 4: Access the Static Website
- In the "Static website hosting" section of my bucket properties, I will see the "Bucket website endpoint" URL. Open a web browser and enter the provided endpoint URL.
![](./img/task%204/1.bucket-website-endpoint.png)

- Verify that MY static website is displayed as expected.
![](./img/task%204/2.access-denied.png)

**Issue Identified:** Access Denied Error on Bucket Website Endpoint URL - When I clicked on the Bucket website endpoint URL to access my static website, I was presented with an "Access Denied" error.

### SOLUTION
**Step one:** Check Bucket Policy:
- In the S3 console, click on my bucket name. Click on "Permissions" tab.
![](./img/SOLUTION/step%201/1.bucket-name-permissions.png)

- Scroll down to the "Bucket policy" section and click "Edit."
![](./img/SOLUTION/step%201/2.bucket-policy-edit.png)

- Write json policy that allows public read access.
![](./img/SOLUTION/step%201/3.write-bucket-policy.png)

- Click "Save changes."
![](./img/SOLUTION/step%201/4.save-changes.png)

- Access the static website using the provided endpoint and verify that it displays correctly.
![](./img/SOLUTION/step%201/5.web-upRUNNING.png)
My static website is now accessible without the "403 Forbidden" error.

### Conclusion
Using Amazon S3 for hosting my static website project highlighted its advantages in simplicity, cost-effectiveness. The detailed documentation of each step, along with the resolution of encountered issues, underscored how S3 simplifies the process of managing and serving static content. This experience demonstrated that Amazon S3 is a robust and efficient solution for hosting static websites, making it an excellent choice for similar projects.