# Portfolio & Resume Workshop
A portfolio and resume workshop with HTML5UP to be hosted on Azure

Written originally for Microsoft Student Partners

## Table of Contents

* Requirements
* Part 1: Setup Code
* [Part 2: Setup Azure and FTP](https://github.com/KaitoKid/PortfolioResumeWorkshop/blob/master/README.md#part-2-setting-up-web-host)
* [Extras for Experts](https://github.com/KaitoKid/PortfolioResumeWorkshop/blob/master/README.md#check-out-your-new-portfolio-online)
* FAQ

## Requirements

1. Download the zip folder containing all of the sample code that you'll need over here: [Sample Code](https://github.com/KaitoKid/PortfolioResumeWorkshop/archive/master.zip)
2. Make sure you have a text editor for code like VSCode, Atom, or Sublime. My recommended is [VSCode](https://code.visualstudio.com/download)
3. Getting an Azure account. Please follow this link, it will only work for 1 hour. **GetAzure**
4. You will need an application called FileZilla over here: [FileZilla Download](https://filezilla-project.org/download.php?type=client)

## Part 1: Setup Code

### Step 1: Open the sample code
1. Extract the folder from the zip file. It should be called `EtherealMSP`.
2. Go into the folder and open up `index.html` with your web browser. You can do this by right clicking it and selecting `Open With`, and choosing your web browser of choice. It should look something like this ![Screenshot of sample](https://i.imgur.com/xGG5Sp5.png)
3. If it does NOT look like the above, something is wrong. Please check the FAQ on common errors, ask a Student Partner, or even your neighbor for help!

### Step 2: Using your text editor
1. Open up your text editor of choice. In my case, I'll be using VSCode.
2. Click on `File` in the top left corner and select `Open`. Browse and locate your `index.html` file.
3. Your editor should now be displaying all of the HTML for the project! ![Editor setup](https://i.imgur.com/KcUmryR.png)

### Step 3: Editing the basic website info
1. Locate the text between the `<title>` tags, on line 7. This is the title of your website that will show up in the tab and for search engines. Change it to your name. ![Title](https://i.imgur.com/WmlYffT.png)
2. If you refresh the page now, it should have the title updated. ![Tab title](https://i.imgur.com/nkhDgBt.png)
3. At the bottom of the page, change the word `Untitled` to your name as well. Leave the `Design` since it's theirs. ![Copyright change](https://i.imgur.com/WYDxMd6.png)

### Step 4: Editing Body Text
1. Each panel on the website is located under the `<!-- Panel -->` in the code. Additionally, each one will be in between `<section></section>` tags. All HTML items and elements are in between tags.
2. Take a look at the text of the `Banner` panel. Can you figure out how to edit the body text? Try using the `<strong></strong>` tag to bold words (stick them in between the tags). A full list of tags that you can try out including italics, strikethrough, etc are available here: [HTML Tags](https://www.w3schools.com/html/html_formatting.asp)
3. Try replacing the image URL with `https://i.imgur.com/guwiBYZ.png` and refreshing the page. ![Change image URL](https://i.imgur.com/NmiJSK9.png)
4. In the next panel `Spotlight`, change the education to match your information. Try adding clubs, sports, or other organizations that you're a part of. Here's a background image for you if you go to UC Berkeley `https://i.imgur.com/mYC0WjI.png`

### Finishing Touches
1. Customize the contact form message to have the personality you want to show.
2. Start scrolling down through the code until you see the section with social media. Change these links to your own. If you don't have them, just delete the line. ![Social media](https://i.imgur.com/5V8y8cI.png)
3. Try changing out some of the images for your own, or adding some more panels! You can see the full list of how to customize it, including buttons, quotes, and more in the bottom of the file.
4. **Delete all the panels you didn't touch after you're done!** They're under the `<!-- Panel -->` tags and in between `<section></section>` tags.

### Bonus
1. To change the spacing and location of elements, try playing with the values of the `span` tag! Further customization can be done through learning HTML and CSS online for free. Try doing a Bing search for them!
2. Want to get the contact form working after learning HTML? Try using this code from [GitHub](https://gist.github.com/ajtroxell/6731408)

## Part 2: Setting up Web Host

For this, there are many ways to host your website, such as through GitHub, your university if they offer it, or many of the website hosting providers online. In this guide, we will cover how to do it on Azure, however these skills are transferrable.

### Activate Your Azure Pass
This can be done following the instructions [here](https://www.microsoftazurepass.com/Home/HowTo). It will take around 5 minutes to complete.

### Create Your Web App

#### Make the app
Click on `New`, select `Web + Mobile` and choose `Web App` ![Deploy web app](https://i.imgur.com/7xr7YAf.png)

#### Name your app
1. Choose a name for your portfolio. You can only use letters, numbers, and dashes 
2. Click on `App Service Plan/Location` and create a new one. ![App name](https://i.imgur.com/DJ5bIOS.png)

#### Change the Service Plan
1. Name your service plan whatever you want, and click on `Pricing Tier`
2. Scroll down to choose the `F1 Free` tier and click `Ok` ![Pricing tier](https://i.imgur.com/xdMCFic.png)
3. Go back, check `Pin to Dashboard` and click `Create`

#### Deploy
Wait for it to deploy! This is your dashboard. ![Waiting for app to deploy](https://i.imgur.com/ehjeW8v.png)

#### Create FTP credentials
1. Your app will automatically open when it's deployed. If it's not, click on it from your Dashboard.
2. Create a username and password through `Deployment credentials` to log into your app. ![Create credentials](https://i.imgur.com/rHAbVf8.png)

#### Find URLs and credentials
Once your credentials are saved, scroll down the sidebar a bit and click on `Properties` ![Created credentials](https://i.imgur.com/oWBuyRy.png)

#### Connect to FileZilla
**Open up FileZilla**. Copy the `FTPS Host Name` into FileZilla, use the `FTP Deplyment User` and password you had just created, and click `Quick Connect` ![FileZilla](https://i.imgur.com/Rf55z7g.png)

#### Trust your own app
Check the box `Always trust certificate` and click `Ok` to login quicker next time. ![Trust](https://i.imgur.com/h223iuc.png)

### Uploading Your Portfolio
1. In FileZilla, the left side is your computer. The right side is your app.
2. Open up the `site` folder on FileZilla and then open up the `wwwroot` folder.
3. Navigate where your project `MSPEthereal` is on the left side.
4. Select all of the files and folder, and `drag + drop` them onto the right side to upload them. ![Copy paste](https://i.imgur.com/nUGzder.png)
5. Now, navigate to your `Yourappname.azurewebsites.net` where your app name is what you had named your app. If you forgot, you can find it under `Properties` in Azure. ![App URL](https://i.imgur.com/03qaGsF.png)

** Congratulations! You've just created your own portfolio! Take a breather and admire your creation **

## Extras for Experts
1. If you want to use your own domain name (i.e. `https://kairui.xyz`) you have to set up a CDN on Azure and point your domain to the nameservers
2. Want to set up HTTPS? Check our CloudFlare for free HTTPS

## FAQ

### 1. My sample code looks like plain text without styles. ![No CSS](https://i.imgur.com/quEuYDs.png)
If it looks like this, you must've not extracted/uploaded the files properly. Please check your folder and file structure again.

### 2. How do I load images from Azure instead of `Imgur`?
Put the image files into the folder `/images` and use the URL `images/myImageName.jpg`. Make sure you have the extension right!

### 3. How much does hosting on Azure cost?
It's free! If you make a CDN and have your own domain name, it'll cost *$1* per *20,000* visitors or so.
