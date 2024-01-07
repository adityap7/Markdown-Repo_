# Hosting a static website using Amazon S3

## About this Tutorial
you can use Amazon S3 to host a static internet site. On a static website, Individual webpages include static content material. they may also include purchaser-aspect scripts.


By contrast, a dynamic website is predicated on server-side processing, consisting of server-side scripts, together with personal home page, JSP, or ASP.net. Amazon S3 does now not aid server-facet scripting, however AWS has different resources for web hosting dynamic websites.

This academic consists of commands and step-via-step walkthroughs to host a static internet site on Amazon S3 bucket. 
## Here is a listing of the steps:
  - Step 1: Create a bucket
  - Step 2: Enable website hosting
  - Step 3: Configure an index document
  - Step 4: Upload the index document while making it public
  - Step 5: Test your website
  - Step 6: Delete your objects and bucket
    
Step 1: Create a bucket
  - 1: Signin into the AWS management Console and search for S3 thru search bar supplied on the top of this page. click on S3 to go to           Amazon S3 dashboard.

    
![S3 Dashboard width-85](https://github.com/adityap7/Markdown-Repo_/assets/6860928/6244c71c-7bcb-4a15-8962-1905ddbe9dcf)
    
  - 2: Select Create bucket.The Create bucket window will open.

![bucket wizard width-85](https://github.com/adityap7/Markdown-Repo_/assets/6860928/60440ef9-7bd5-41c7-8d7c-003eff624acf)

  - 3: In Bucket name, enter a DNS-compliant name in your bucket.

    [] The bucket call need to:
    
  ```
    > Be specific across all of Amazon S3.
    > Be among 3 and sixty three characters lengthy.
    > Not incorporate uppercase characters.
    > Start with a lowercase letter or range.
  ```

![Bucket Name](https://github.com/adityap7/Markdown-Repo_/assets/6860928/76571e99-237b-4a2a-b0a6-cd795a37dc26)

  - 4: In Region, choose the AWS Region where you want the bucket to reside.
    
![AWS Region](https://github.com/adityap7/Markdown-Repo_/assets/6860928/b78d4832-569f-4142-af30-e31e752dc1d2)

  - 5: Under Object Ownership, enable ACLs by selecting "ACLs enabled" and control ownership of objects uploaded in your bucket by               selecting "Bucket owner preferred".
       This ensures that the bucket owner owns and has full control over new objects that other accounts write to the bucket with                the bucket-owner-full-control canned ACL.

![Object Ownership](https://github.com/adityap7/Markdown-Repo_/assets/6860928/afebb1f2-f929-44ab-9f47-641965b0c5d1)

    
