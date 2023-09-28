# AppleMail.Signiture

### A repo for your custom build Apple.Mail signature.

Knowing the basics of software developemnt and how to access commands and controls can take you to some strange places. I had this issue recently trying to create a 'signature' with the Mail App on my Macbook.

There are various websites that allow you to create signatures that can be added to your signature selector in the App. A problem arrises when you come to import them, however. They never seem to work correctly once imported, be it links broken, styles not working and layout going bananas! 🍌

Many of these services then offer a <code>Premium</code> subscription which allows the code to work in more platforms and the options to add more styles. **No thanks!** 

It took some time, but I figured a way to access the 'signatures' files directly, then import my own custom <code>HTML</code> code for each file, then lock the files so that the text compiler in the Mail App doesn't try to warp the code.

Follow the instructions below to make your own...!

<span></span>

<img src="./Me_Sig_1.png" height="160"/>

## Step 1

### Create a new Signature

<ul>
<li>In Apple Mail, open <code>Settings...</code> > <code>Signatures</code>.</li>
<li>Select your email account in the left column.</li>
<li>Now create a new signature by clicking on <code>+</code> icon.</li>
<li>Name the new Signature 'NEW_SIGNATURE'.</li>
<li>Make sure the <code>Always match my default font</code> checkbox is <code>off</code>.</li>
<li>Close the <code>Settings</code> window then close Apple Mail by right-clicking on the screen bottom Icon and selecting <code>Quit</code>.</li>
</ul>
<img src="./Assets/1.png" width="350"/>

## Step 2

### Open a new TextEdit doc

<ul>
<li>Use the spotlight search function on your Mac: <code>Command</code> + <code>Spacebar</code>.</li>
<li>Type <code>TextEdit</code> and press <code>Enter</code> to open it.</li>
<li>In TextEdit, select <code>New Document</code> to open a new file.</li>
<li>Select <code>TextEdit</code> > <code>Preferences...</code> in the top menu.</li>
<li>Navigate to the <code>Open and Save</code> section.</li>
<li>Make sure that the <code>Display HTML files as HTML code instead of formatted text</code> option is checked.</li>
<li>Close the <code>Preferences</code> window.</li>
</ul>
<img src="./Assets/2.png" width="350"/>

### This is where the magic happens!...

*The next step will locate our new signature file from the Apple Mail App. Now, it must be stated that Apple has dileberatly made these files private so they wont appear in your regular <code>Finder</code> searches. This is beacuase the enclosed files are not meant to be editable by regular users for fear of writing bugs in the App can't read!*

## Step 3

### Locate and Open the hidden 'NEW_SIGNATURE' file

<ul>
<li>Navigate to your home desktop screen and select the <code>Go</code> drop-down menu, then <code>Go to Folder</code>.</li>
<li>Type <code>~/Library/Mail/V10/MailData/Signatures</code> into the search window and press Enter.</li>
<li>In the new (hidden) folder, you should see several files that hold your Signatures. Right-click on each and choose <code>Open with</code> > <code>TextEdit</code>.</li>
</ul>
<img src="./Assets/3.png" width="350"/>
<ul>
<li>The file we want should have '>NEW_SIGNATURE<' at the bottom within the <body> tags.
Go ahead and delete the entire <body> tags and everything in it, leaving just the top Content and Version information at the top.</li>
</ul>
<img src="./Assets/5.png" width="350"/>

## Step 4

### Create the New Design and Test it

<ul>
<li>Paste your custom design into the Signature file in HTML format.</li>

***...You can find 5 different designs in my <code>Example_Signatures.FromNick</code> folder***

<li>Remove the <code>< DOCTYPE ></code> and the <code><code html ></code> tags - Top and bottom!</li>
</ul>
<img src='./Assets/6.png' width="350">
<ul>
<li>Close the <code>TextEdit</code> app and in the 'hidden' Signatures folder, right click the same file and select <code>Get info</code> </li>
<li>This will open a new window for the file details. Make sure the <code>Locked</code> box is ticked ✅ </li>
</ul>
<img src="./Assets/7.png" width="200" alt="Image description"/>
<ul>
<li>Then, open up your Apple Mail App again and click to create a new email</li>
<li>The <code>NEW_SIGNATURE</code> should be there and will now render your new footer to the bottom of the page!</li>
</ul>

# That's it! 

If this has helped. Please <code>Follow</code> and let me know by reaching out!

Thanks.


[Click here to connect via LinkedIn!](https://www.linkedin.com/in/nicholas-valente-electrics/)