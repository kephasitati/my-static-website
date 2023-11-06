# my-static-website
This repository contains a demo website built from an AWS LABS template for a static website, hosted on Amazon S3. Explore the website's content, which serves as a demonstration of AWS's capabilities for hosting static web content

Amazon S3 Static Website Setup
Table of Contents
Task 1: Creating a Bucket in Amazon S3
Task 2: Uploading Content to Your Bucket
Task 3: Enabling Access to the Objects
Task 4: Updating the Website
Task 1: Creating a Bucket in Amazon S3
In this task, I created an Amazon S3 bucket and configured it for static website hosting.

Log in to the AWS Management Console.

Go to the Services menu and select S3.

Choose "Create bucket."

Note: The bucket name must be globally unique, and it is shared among all AWS accounts. Be sure to select a unique name. For this lab, you can use a bucket name like "website-123" (my-website-321).
Configure the bucket as follows:

Bucket name: my-website-321
Verify the AWS Region is set to us-east-1.
Under Object Ownership, select ACLs enabled and verify that Bucket owner preferred is selected.
Clear "Block all public access," acknowledging that the current settings may make the bucket and objects public.
Choose "Create bucket."

I used tags to add additional information to the bucket, such as Department: Marketing.

The bucket is now configured for static website hosting.

Task 2: Uploading Content to Your Bucket
In this task, you will upload the files that serve as your static website to the bucket.

Download the required DEMO files: index.html, script.js, style.css.
Return to the Amazon S3 console and select the bucket you created earlier.
Choose the "Objects" tab.
Click "Upload" and add the downloaded files.
If prompted, choose to acknowledge that existing objects with the same name will be overwritten.
Choose "Upload."
Your website files are now in the bucket.

Task 3: Enabling Access to the Objects
By default, objects in Amazon S3 are private. In this task, you will make the uploaded objects publicly accessible.

Confirm that the objects are private by refreshing the browser tab showing the 403 Forbidden message.
You should still see a 403 Forbidden message. This is expected, as the content is private.
Make the objects public by selecting all three objects, going to the Actions menu, and choosing "Make public via ACL."
Your static website is now publicly accessible.
Task 4: Updating the Website
You can change the website by editing the HTML file and uploading it again to the S3 bucket.

Edit the index.html file by replacing "Served from Amazon S3" with "Created by <YOUR-NAME>" (substitute your name for <YOUR-NAME>).
Save the file.
Return to the Amazon S3 console and upload the edited index.html file.
Select index.html and choose the "Make public via ACL" option again.
Return to the web browser tab with the static website and refresh the page.
Your name should now be on the page.
The static website is now accessible on the internet, hosted on Amazon S3.
