# What is Firing Range?

Firing Range is a test bed for web application security scanners,
providing synthetic, wide coverage for an array of vulnerabilities.

It can be deployed as a Google App Engine application. A public instance
is running at https://public-firing-range.appspot.com.

# Google Compute Engine Installation Instructions

1. `sudo apt-get install -y git ant unzip google-cloud-sdk-app-engine-java`
1. Download the Appengine SDK for Java from
   http://cloud.google.com/appengine/downloads and unzip it in a directory.
   If the current version of Appengine SDK is 1.9.77, then you can use the following commands: <br/>
   `wget https://storage.googleapis.com/appengine-sdks/featured/appengine-java-sdk-1.9.77.zip` <br/>
   `unzip appengine-java-sdk-1.9.77.zip`
1. `git clone https://github.com/ashishin/firing-range.git`
1. `cd firing-range`
1. `ant runserver -DappengineSdk=../appengine-java-sdk-1.9.77`

The application then will be run on port 8080 on Google Compute Engine. Make sure to add firewall rule for port 8080.

# License information

See the LICENSE file.
