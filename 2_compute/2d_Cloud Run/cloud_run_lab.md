### Cloud Run Commands  

From - https://cloud.google.com/run/docs/quickstarts/build-and-deploy   

To update gcloud components  
`gcloud components update` 

To create the sample application  
`mkdir helloworld-python`
`cd helloworld-python`

To build locally and push using Docker  
`docker build . --tag gcr.io/[PROJECT-ID]/[IMAGE]`  
NOTE: requires config Docker to use GCR  
`gcloud auth configure-docker`  

To push to GCR from local build  
`docker push gcr.io/[PROJECT-ID]/[IMAGE]`  

--OR--

To build and push the image using Cloud Build to GCR  
`gcloud builds submit --tag gcr.io/[PROJECT-ID]/helloworld`

To deploy the image to Cloud Run  
`gcloud run deploy --image gcr.io/[PROJECT-ID]/helloworld`

To list the services  
`gcloud run services list`

To test the deployment  
- open the service URL in a browser

To clean up  
- delete the Cloud Run instance
- delete the image from Google Container Registry  