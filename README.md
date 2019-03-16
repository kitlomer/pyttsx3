# pyttsx3

import pyttsx
import pywin32

engine = pyttsx.init()
voices = engine.getProperty('voices')

engine.setProperty('voice', voices[1].id) #change index to change voices
engine.say('I\'m a little teapot...')

engine.runAndWait()
