# gui-cucfrom tkinter import *
from tkinter import messagebox


class Gui:
    def __init__(self):
        self.main_GUi = Tk()
        self.main_GUi.title('Ahmed GUI')
        self.main_GUi.minsize(300, 300)
        self.label = Label(self.main_GUi, text='Enter num1')
        self.label.pack()
        self.entry = Entry()
        self.entry.pack()
        self.labe2 = Label(self.main_GUi, text='Enter num2')
        self.labe2.pack()
        self.entry2 = Entry()
        self.entry2.pack()
        self.btn = Button(self.main_GUi, text='ADD', command=self.do)
        self.btn.pack()
        self.main_GUi.mainloop()

    def do(self):
        num1 = int(self.entry.get())
        num2 = int(self.entry2.get())
        total = num1+num2
        self.label3 = Label(
            self.main_GUi, text='the result will be'+str(total))
        self.label3.pack()


Gui()
