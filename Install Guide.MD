The website is designed to be able to require very little to no backend and is open source. As such the entire site is downloadable and can be deployed to work from your local machine to work from your personal computer, or can be installed to a basic local or hosted web server for your own or your group's ease of access.

* No need for SQL/database backend.
* Powerful n' Portable

The most current version of this document is found [here](https://wiki.5e.tools/index.php?title=5eTools_Install_Guide)
<br />

## **PC Install** ( Simple/ Local Install)
This is for running the code from your local PC (This will require internet access to run various libraries, and pull images etc. - and you will need to run a local webserver)

<br />
👉 Go to [get.5e.tools](http://get.5e.tools) and choose an installation set (see below for which option best suits you)

👉 Confirm you are going to be using a [**supported browser**](https://wiki.5e.tools/index.php/Template:Supportedbrowserversion)

<br />

Download the **5eTools** (non development) archive/zipped code from the [**download site**](http://get.5e.tools).

Uncompress the files into a folder.

Launch the Webserver (see below) and open 5eTools.html in the root of the unzipped files using a [**supported browser**](https://wiki.5e.tools/index.php/Template:Supportedbrowserversion)

<br/>

**FOR MOBILE**
 See [*below*](https://wiki.5e.tools/index.php/5eTools_Install_Guide#Mobile_Platform_Installation_.28beta_.2F_not_offically_supported.29)

<br/>

### Installing for use without Internet Access

 **FOR PC**

👉 Make sure you've downloaded the **5eTools development files**.

👉 You'll also need the **Images** zip.

* Uncompress the **Images** zip into the same folder as the **5eTools development files**.

* You may want to edit the source to remove links back to 5eTools/Homebrew.

* You can choose to AUTOMATICALLY load specific homebrew files (see below).

 * Copy the 5eTools.html and rename the copy to index.html

* Launch the Webserver (see below) and open localhost / 5eTools.html in the root of the unzipped files using a [**supported browser**](https://wiki.5e.tools/index.php/Template:Supportedbrowserversion).

<br />

### Local Web Server

#### Python

* install the latest [**python**](https://www.python.org/downloads/) (preinstalled on Mac)

* open terminal (command prompt)

* Navigate to the directory you unzipped 5eTools in the terminal window.

* type <code>py -m http.server</code> 

  * you may also specify *SimpleHTTPServer* ie <code>py -m SimpleHTTPServer</code>

  * you may also specify a *port* at the end of the command ie either <code>py -m SimpleHTTPServer 8080</code> or <code>py -m http.server 8080</code> 

(if you specify a port other than 80, you will need to include that in your URL eg. in the example above you'd need to use <code>http://localhost:8080</code>

</div>

#### Devd

* Install [**devd**](https://github.com/cortesi/devd#install)

* open terminal (command prompt)

* Navigate to the directory you unzipped 5eTools in the terminal window.

* type <code>devd.exe -ol .</code>

* open 5eTools.HTML

<br>

#### Wampserver

**Step 1: Download WampServer**

Installing all the individual pieces of software you need and configuring them to work together can be daunting. WampServer is a software package that can do almost all of this for you: it installs Apache, PHP, and MySQL, and provides a simple interface to use them.

* Navigate to http://www.wampserver.com/en.
* Click the word "download" at the top of the page.
* Click the WampServer version you need. (There are several versions with subtle differences that you should not need to worry about; just look at the first two options on top. If you know you have 64-bit Windows, click the 64-bit version; otherwise, click the 32-bit version.)
* Actually getting the installer to download can be confusing, because (as of March 2014) this portion of the website is glitchy and partly in French. Look for the small link labeled "you can download it directly" at the top of the popup and click it. You should be taken to a SourceForge page that will automatically start downloading the installer.

You should not need to worry about any of the warnings on the popup, except perhaps for the first one (about the Visual C++ runtime.) The Visual C++ runtime is a standard piece of software that is required to run many programs, so your computer probably already has it. If WampServer will not run, however, you may need to come back to this step and install it - just follow one of the links in the first warning (depending on whether you have 32-bit or 64-bit Windows) to download and install it.
<br/>

*Note*: Although you need several hundred megabytes of free space to run the software, the actual installer is only about 35 MB.
<br/>

**Step 2: Install WampServer**

* Run the installer you just downloaded.
* You can leave all the options on their defaults and just click through it, but stop when you get to the page titled "Select Destination Location." '''This page is important'''. After you install WampServer, you will have to put all the files you want the server to "see" in a special folder inside the one you're selecting in this step. Therefore, you want to install WampServer somewhere you can easily access. This is a matter of personal preference, but you may prefer to change the install location to somewhere like a subfolder of your Documents folder.
* Once you're happy with where WampServer will install, click through the rest of the installer.


<br/>

### Video Instruction

https://www.youtube.com/watch?v=lE6Y6M9xPLw

<br/>


### Hosted Server Install

#### [InMotion Hosting](https://www.inmotionhosting.com/support/website/getting-started-guides/where-to-upload-files)

#### [Bluehost](https://my.bluehost.com/hosting/help/upload-site)

#### [GoDaddy](https://www.godaddy.com/help/upload-your-website-files-in-cpanel-hosting-16068?)

<br/>

<br/>

## Mobile Platform Installation (beta / not offically supported)

**FOR MOBILE (online)**
 Bring up the 5e.tools site.

* Click/Accept the Add 5eTools to Home screen

 *This preloads all the data locally. Images still pull from external sources.*

<br/>

## FOR MOBILE (offline)

#### Android

<br/>
 
1️⃣ Install the app (https://play.google.com/store/apps/details?id=com.esminis.server.apache), take note of the "data directory path" (likely a folder name htdocs in the root of internal storage) and start the server once so that the app creates the necessary files on your device. Take note of the port where the webserver is running (likely 8000).

2️⃣ Move the extracted files from the 5etools zip into the public folder inside of your "data directory path" (e.g. htdocs/public)

3️⃣ With browser (Chrome/Firefox) point to the server with ''http://localhost/:<port>/5etools.html'' or whatever page you need.

----

#### iPhone/iOS

<br/>

1️⃣ On the iPhone, go to Settings → Safari → Advanced and activate the switch “web inspector”:

2️⃣ Connect the phone to your MacBook using a lightning-to-USB cable.

3️⃣ On the MacBook, open up Safari and go to Develop → {NAME_OF_YOUR_IPHONE} and select “Connect via Network”:

4️⃣ Open up a terminal and run the command “ifconfig” to see the list of current network interfaces and take note of the IP address of the last entry in the list:

5️⃣ On your phone, in Safari, use the IP address to access your locally running website. For example, if you use create-react-app, instead of going to http://localhost:3000, with the IP I got here, the address to use is http://169.254.145.56:3000 (don’t forget the http:// prefix):
