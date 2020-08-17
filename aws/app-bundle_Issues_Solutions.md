### Potential issues configuring ngxinx and uploading app bundle to Elastic Beanstalk:

-Ensure JAR in Procfile is the original JAR name (before it's renamed to application.jar)
-Use .platform for configuring Amazon Linux 2, .ebextensions is for AMI
-File structure is .platform/nginx/conf.d/<configuration_file.conf>
-Ensure end of .conf file is semicolon
-Ensure app bundle is zipped properly, had an issue with tar, used WinRAR