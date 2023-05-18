Postmortem

Logging into my webserver for ALX's System Engineering & DevOps project 0x1A at approximately 06:00 West African Time (WAT) here in Nigeria, an outage occurred on an isolated Ubuntu 20.04 container running an Apache web server. Webserver was  returning an unknown error,502.

Debugging Process



• Checked running processes using ps aux. Two apache2 processes - root and www-data - were properly running.

• check the server logs to see if there are any errors that can help me identify the issue. The logs didn't provide any clues
•  I restarted the server and boom....the error was rectified.  


Summation

Using "sudo  reboot" restarted the server and cleared the error 502 'unknown error '

Prevention

Sometimes, a simple restart of the server can resolve the issue. This is especially true if the server has been running for a long time and has not been restarted recently


