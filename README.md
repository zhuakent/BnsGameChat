# BnsGameChat
Blade &amp; Soul Game Chat Assistant to help non-native player in communication

This program uses Pcap.Net to capture the message arrived at your PC and decode it to a readable form as you see it at the Game chat. You don't have to change the IP address if you are playing on the Taiwanese server. It work with the NA server, but you need to change the IP address or capture port of the server.->IP 64.25.37.253 or Port: 10241. Not tested on other server but I think it should work.

As this is written in WPF, to sendkeys, InputSimulator is used to make my life easier. You can input the text onto the editable ComboBox and send the message to the chat box of the game. The message will be sent to the current default Chat Channel. To send the message to a different chat channel, used the Game Chat command. Example to send to faction channel :"/f your message" or to region "/z your message".

As I am a non-native player, I find it difficult to communicate in Chinese especially in the Traditional Chinese. Google web translation is used to help me in the translation between language. As thie is not using the Google API, please refrain from using it too often or you may be locked out for a time period. An alternative is to used the cut and paste function provided by the combobox.  There is also a custom list of the commonly used phrases that can be customized. Go to the program directory and edit the custom.txt file, put in your custom text and reload it. The custom list appear on the dropdown of the combobox.  
If your purpose is just for sending messages, you don't have to turn on the Chat capture.

The program allow you to save a log file, cap at 512Kbytes. Once it exceeded the cap limit, the old file will be renamed and a new files: log.txt is created. However, the program only detect the file size when you click on Log file command. As a precaution, please don't log it and let it run forever as the file can get very large.

As this is not a clientless program, the game client must be running. I wish that I can do a clientless one but I have yet to know how to do it. However, you can send messages when the Game client is minimize.

For more information, please look at the screenshots in the image folder, you should be able to undertstand it as this is a very simple and straightforward program.

# Unresolve Problem
For basic communication, it worked fine. However, there are problem that I am unable to resolve. Like example, when there is a link to items or dungeon, it appear as "link id='item-name:32cfd5.1.2'/" or "link id='raid-dungeon:raid_AkTaeHoo_LightRaid_02'/".  Unless I know where it is linked to, I don't think I could do anything.

When you are at F8, wow! There are some part of the message that I have yet to decode. Most of the messages are used by the system to track your position, the channel, the dungeon , your party etc. I can remove those but I decided to leave it there.

In the meantime, have fun! Any suggestion or feedback is welcome!
