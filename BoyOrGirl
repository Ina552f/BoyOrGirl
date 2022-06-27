from kivy.app import App
from kivy.uix.gridlayout import GridLayout
from kivy.uix.label import Label
from kivy.uix.image import Image
from kivy.uix.button import Button
from kivy.uix.textinput import TextInput
import random


class BoyOrGirl(App):
    def build(self):        
        self.window = GridLayout()
        self.window.cols = 1

        #add widgets to window
        self.window.add_widget(Image(source="RLogo.png"))
        # change background to white since pic is not vector

        self.question = Label(text="Dreng eller pige?")
        self.window.add_widget(self.question)

        
        self.button = Button(text="Guess")
        self.button.bind(on_press=self.callback)
        self.window.add_widget(self.button)
        return self.window


    def callback(self, instance):
        gender = random.choice(('male', 'female'))

      #  self.question.text = (("Du får en " + text=gender + "!"
      #  self.window.add_widget(Label(text=gender))

        self.window.add_widget(Label(text=gender))
        print(gender)


if __name__ == "__main__":
    BoyOrGirl().run()
