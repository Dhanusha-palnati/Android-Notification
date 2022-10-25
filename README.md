# Android-Notification
from kivy.app import App
from kivy.uix.button import Button
import plyer

class telegram(App):
    def build(self):
        return Button(text='telegram', on_press=self.notify)

    def notify(self, obj):
        plyer.notification.notify(title="techsnap", messsage="welcome")

telegram().run()
