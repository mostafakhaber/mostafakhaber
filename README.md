- 👋 Hi, I’m @mostafakhaber
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
mostafakhaber/mostafakhaber is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
from kivy.app import App
from kivy.uix.boxlayout import BoxLayout
from kivy.uix.label import Label

class StudentApp(App):
    def build(self):
        layout = BoxLayout(orientation='vertical')
        students = ["Studente 1", "Studente 2", "Studente 3"]

        for student in students:
            label = Label(text=student, font_size='20sp')
            layout.add_widget(label)

        return layout

if __name__ == '__main__':
    StudentApp().run()
