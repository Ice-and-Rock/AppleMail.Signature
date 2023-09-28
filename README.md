# AppleMail.Signiture
A repo for your custom build Apple.Mail signature.

Knowing the basics of software developemnt and how to access commands and controls can take you to some strange places. I had this issue recently trying to create a 'signature' with the Mail App on my Macbook. 

There are various websites that allow you to create signatures that can be added to your signature selector in the App. The problem arrises when you come to import them, however. They never seem to work correctly once imported, be it links broken, styles not working and layout going bananas! 🍌 

It took some time, but I figured a way to access the 'signatures' files directly, then import my own custom HTML code for each file, then lock the files so that the text compiler in the Mail App doesn't try to warp the code!

Follow the instructions below to make your own...! 


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
<img src="./1.png">

## Step 2
### Open a new TextEdit doc
<ul>
<li>
Use the spotlight search function on your Mac: <code>Command</code> + <code>Spacebar</code>.
</li>
<li>
Type <code>TextEdit</code> and press <code>Enter</code> to open it.
</li>
<li>
In TextEdit, select <code>New Document</code> to open a new file.
</li>
<li>
Select <code>TextEdit</code> > <code>Preferences...</code> in the top menu.
</li>
<li>
Navigate to the <code>Open and Save</code> section.
</li>
<li>
Make sure that the <code>Display HTML files as HTML code instead of formatted text</code> option is checked.
</li>
<li>
Close the <code>Preferences</code> window.
</li>
</ul>
<img src="./2.png"/>


### This is where the magic happens!...
The next step will locate our new signature file from the Apple Mail App. Now, it must be stated that Apple has dileberatly made these files private so they wont appear in your regular <code>Finder</code> searches. This is beacuase the enclosed files are not meant to be editable by regular users for fear of writing bugs in the App can't read!

## Step 3
### Locate and Open the hidden 'NEW_SIGNATURE' file
<ul>
<li>
Navigate to your home desktop screen and select the <code>Go</code> drop-down menu, then <code>Go to Folder</code>.
Type <code>~/Library/Mail/V10/MailData/Signatures</code> into the search window and press Enter.
</li>
<li>
In the new (hidden) folder, you should see several files that hold your Signatures. Right-click on each and choose <code>Open with</code> > <code>TextEdit</code>.
</li>
  <img src="./3.png"/>
<li>
The file we want should have '>NEW_SIGNATURE<' at the bottom within the <body> tags.
Go ahead and delete the entire <body> tags and everything in it, leaving just the top Content and Version information at the top.
</li>
</ul>
<img src="./5.png"/>


<div style="display: flex;">
  <div style="flex: 1; padding-right: 20px;">
    <h2>Step 4</h2>
    <h3>Create the New Design and Test it</h3>
    <ul>
      <li>Paste your custom design into the Signature file in HTML format.</li>
      <li>Remove the &lt;!DOCTYPE html&gt; and the &lt;html&gt; tags - Top and bottom!</li>
      <li>Close the <code>TextEdit</code> app and in the 'hidden' Signatures folder, right-click the same file and select <code>Get info</code>.</li>
      <li>This will open a new window for the file details. Make sure the <code>Locked</code> box is ticked ✅</li>
      <li>Then, open up your Apple Mail App again and click to create a new email.</li>
      <li>The <code>NEW_SIGNATURE</code> should be there and will now render your new footer to the bottom of the page!</li>
    </ul>
  </div>
  <div style="flex: 1;">
    
    <img src="./7.png" width="100" alt="Image description" />
  </div>
</div>
