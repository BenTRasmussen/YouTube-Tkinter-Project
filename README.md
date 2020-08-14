# YouTube-Tkinter-Project
Small Tkinter Project Built in YouTube.


Hello eveyone this is a free example file for the tkinter project we worked on in a youtube video.



import tkinter as tk
from tkinter import *

#Init window
win = tk.Tk()
win.title("My App")
win.geometry("500x600")
win.resizable(width=False, height=False)


#Creates a text node
Label = tk.Label(win, text="Welcome To My App", fg="red")
Label.pack()

Entry = tk.Entry(win, bg="yellow")
Entry.pack()

def startTest():
    newText = Entry.get()
    NewLabel = tk.Label(win, text=newText, fg="green").pack()




button = tk.Button(win, text="Test", fg="green", command=startTest)
button.pack()

#Keeps the window running
win.mainloop()
