Here is the project part of CI/CD 
1. With groovy  created pipeline which is build the image with dockerfile 
2. Uploaded the custom image to "docker hub " 
3. There is build 2 type of pipelines : (with ssh connection and the second one with node)
   (in github the webhook is configured and after the push request received  in mentioned repo the jenkins job triggered)
4. Then with ssh  jenkins connected  to the worker node check if the container is exist or not and then deployed the application to avoid the failures)
5. Then remove the custom created image from jenkins server.
