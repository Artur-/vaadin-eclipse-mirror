In situations where you need to be able to install Vaadin Eclipse Plug-ins w/o access to the main update-site ("offline"), you can create a mirror containing all the dependencies needed to install Vaadin Plug-in for Eclipse and Vaadin Designer.

# Create mirror

First clone this project, then run

```mvn package```

# Install

`target/vaadin-update-site` now contains the update-site. You can serve this from your own server, or use it as a local update-site.

In Eclipse

 1. Help -> Install New Software
 2. Click "Add..."
 3. http://your.server.ip/path/to/vaadin-update-site OR press "Local..." if you have the site locally on your computer
 4. Check "Apache Ivy library" and "Vaadin"
 5. Uncheck "Contact all update sites [...]"
 6. Click "Finish" and restart Eclipse when prompted
