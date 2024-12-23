# Website_opener_pyttsx3
# Using python to open a website
import pyttsx3
import webbrowser 
import getpass
engine = pyttsx3.init()
engine.say("sir , given below are the website you want to open , choose one from it ")
engine.runAndWait()
print("youtube,","Hotstar,","prime,","Chatgpt,") # enter your website names here
engine.say("After entering the , pass , enter your website name")
engine.runAndWait()
def open_websites():
    x = getpass.getpass("Enter your pass")
    if "Hari@123" in x:
        z = input("Enter the website name :""")
        if "youtub" in z:
            url = "https://www.youtube.com/"
            webbrowser.open(url)
    
        if "hotstar" in z:
            url = ""
            webbrowser.open(url)
    
        if "prime" in z:
            url = ""
            webbrowser.open(url)
    
        if "Chat gpt" in z:
            url = ""
            webbrowser.open(url)
    else:
        engine.say("your , pass is wrong")
        engine.runAndWait()
       
open_websites()
   
