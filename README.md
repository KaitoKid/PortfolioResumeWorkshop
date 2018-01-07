# Portfolio & Resume Workshop
A portfolio and resume workshop with HTML5UP to be hosted on Azure

## Requirements

1. Download the zip folder containing all of the sample code that you'll need over here: [Sample Code](https://github.com/KaitoKid/PortfolioResumeWorkshop/archive/master.zip)
2. Make sure you have a text editor for code like VSCode, Atom, or Sublime. My recommended is [VSCode](https://code.visualstudio.com/download)
3. Getting an Azure account. Please follow this link, it will only work for 1 hour. [Azure Pass Claim](https://getazure.com)
4. You will need an application called FileZilla over here: [FileZilla Download](https://filezilla-project.org/download.php?type=client)

## Setup Code

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
3. At the bottom of the page, change the word `Untitled` to your name as well. Leave the `Design` since we're using their template. ![Copyright change](https://i.imgur.com/WYDxMd6.png)

### Step 4: Editing Body Text
1. Take a look at the text of the `Banner` panel. Can you figure out how to edit the body text? Try using the `<strong></strong>` tag to bold words (stick them in between the tags). A full list of tags that you can try out including italics, strikethrough, etc are available here: [HTML Tags](https://www.w3schools.com/html/html_formatting.asp)
2. Try replacing the image URL with `https://i.imgur.com/guwiBYZ.png` and refreshing the page. ![Change image URL](https://i.imgur.com/NmiJSK9.png)
3. In the next panel `Spotlight`, change the education to match your information. Try adding clubs, sports, or other organizations that you're a part of. Here's a background image for you if you go to UC Berkeley `https://i.imgur.com/mYC0WjI.png`

### Finishing Touches
1. Customize the contact form message to have the personality you want to show.
2. Start scrolling down through the code until you see the section with social media. Change these links to your own. If you don't have them, just delete the line. ![Social media](https://i.imgur.com/5V8y8cI.png)
3. Try changing out some of the images for your own, or adding some more panels! You can see the full list of how to customize it, including buttons, quotes, and more in the bottom of the file. *Delete them when you're done!*
4. To change the spacing and location of elements, try playing with the values of the `span` tag! Further customization can be done through learning HTML and CSS online for free. Try doing a Bing search for them!
5. Want to get the contact form working after learning HTML? Try using this code from [GitHub](https://gist.github.com/ajtroxell/6731408)

## Part 2: Setting up Azure

### Activate Your Azure Pass
This can be done following the instructions [here](https://www.microsoftazurepass.com/Home/HowTo). It will take around 5 minutes to complete.

### Create Your Web App

### Connect to App With FileZilla

## FAQ

### 1. My sample code looks like plain text without styles. ![No CSS](https://i.imgur.com/quEuYDs.png)
If it looks like this, you must've not extracted/uploaded the files properly. Please check your folder and file structure again.

### 2. How do I load images from Azure instead of `Imgur`?
Put the image files into the folder `/images` and use the URL `images/myImageName.jpg`. Make sure you have the extension right!
