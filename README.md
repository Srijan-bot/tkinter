# tkinter
import tkinter
from tkinter import *
from tkinter import  messagebox as msg
from tkinter import filedialog


root=tkinter.Tk()

root.iconbitmap("tic.ico")
winner=" "
root.resizable(0,0)
root.config(bg="light blue")

def newgame():
    restart()
    pointo.set(0)
    pointx.set(0)

def deactivate():
    b1.config(state=DISABLED)
    b2.config(state=DISABLED)
    b3.config(state=DISABLED)
    b4.config(state=DISABLED)
    b5.config(state=DISABLED)
    b7.config(state=DISABLED)
    b8.config(state=DISABLED)
    b9.config(state=DISABLED)

def check_if_winner():
    global winner
    if b1["text"]=="X" and b2["text"]=="X" and b3["text"]=="X":
        b1.config(bg=  "powder blue")
        b2.config(bg=  "powder blue")
        b3.config(bg=  "powder blue")
        msg.showinfo("TIC TAC TOE","Congratulation!,X won the game")
        winner="X"
        check_score()   
        deactivate()
        restart()
    elif b4["text"]=="X" and b5["text"]=="X" and b6["text"]=="X":
        b4.config(bg=  "powder blue")
        b5.config(bg=  "powder blue")
        b6.config(bg=  "powder blue")
        msg.showinfo("TIC TAC TOE","Congratulation!,X won the game")
        winner="X"
        check_score()
        deactivate()
        restart()


    elif b7["text"]=="X" and b8["text"]=="X" and b9["text"]=="X":
        b7.config(bg=  "powder blue")
        b8.config(bg=  "powder blue")
        b9.config(bg=  "powder blue")
        msg.showinfo("TIC TAC TOE","Congratulation!,X won the game")
        winner="X"
        check_score()
        deactivate()
        restart()

    elif b1["text"]=="X" and b4["text"]=="X" and b7["text"]=="X":
        b1.config(bg=  "powder blue")
        b4.config(bg=  "powder blue")
        b7.config(bg=  "powder blue")
        msg.showinfo("TIC TAC TOE","Congratulation!,X won the game")
        winner="X"
        check_score()
        deactivate()
        restart()

    elif b2["text"]=="X" and b5["text"]=="X" and b8["text"]=="X":
        b2.config(bg=  "powder blue")
        b5.config(bg=  "powder blue")
        b8.config(bg=  "powder blue")
        msg.showinfo("TIC TAC TOE","Congratulation!,X won the game")
        winner="X"
        check_score()
        deactivate()
        restart()

    elif b3["text"]=="X" and b6["text"]=="X" and b9["text"]=="X":
        b3.config(bg=  "powder blue")
        b6.config(bg=  "powder blue")
        b9.config(bg=  "powder blue")
        msg.showinfo("TIC TAC TOE","Congratulation!,X won the game")
        winner="X"
        check_score()
        deactivate()
        restart()

    elif b1["text"]=="X" and b5["text"]=="X" and b9["text"]=="X":
        b1.config(bg=  "powder blue")
        b5.config(bg=  "powder blue")
        b9.config(bg=  "powder blue")
        msg.showinfo("TIC TAC TOE","Congratulation!,X won the game")
        winner="X"
        check_score()
        deactivate()
        restart()

    elif b3["text"]=="X" and b5["text"]=="X" and b7["text"]=="X":
        b3.config(bg=  "powder blue")
        b5.config(bg=  "powder blue")
        b7.config(bg=  "powder blue")
        msg.showinfo("TIC TAC TOE","Congratulation!,X won the game")
        winner="X"
        check_score()
        deactivate()
        restart()

#_______________________
    elif b1["text"]=="O" and b2["text"]=="O" and b3["text"]=="O":
        b1.config(bg=    "powder cyan")
        b2.config(bg=    "cyan")
        b3.config(bg=    "cyan")
        msg.showinfo("TIC TAC TOE","Congratulation!,O won the game")
        winner="O"
        check_score()
        deactivate()
        restart()

    elif b4["text"]=="O" and b5["text"]=="O" and b6["text"]=="O":
        b4.config(bg=    "cyan")
        b5.config(bg=    "cyan")
        b6.config(bg=    "cyan")
        msg.showinfo("TIC TAC TOE","Congratulation!,O won the game")
        winner="O"
        check_score()
        deactivate()
        restart()

    elif b7["text"]=="O" and b8["text"]=="O" and b9["text"]=="O":
        b7.config(bg=    "cyan")
        b8.config(bg=    "cyan")
        b9.config(bg=    "cyan")
        msg.showinfo("TIC TAC TOE","Congratulation!,O won the game")
        winner="O"
        check_score()
        deactivate()
        restart()

    elif b1["text"]=="O" and b4["text"]=="O" and b7["text"]=="O":
        b1.config(bg=    "cyan")
        b4.config(bg=    "cyan")
        b7.config(bg=    "cyan")
        msg.showinfo("TIC TAC TOE","Congratulation!,O won the game")
        winner="O"
        check_score()
        deactivate()
        restart()

    elif b2["text"]=="O" and b5["text"]=="O" and b8["text"]=="O":
        b2.config(bg=    "cyan")
        b5.config(bg=    "cyan")
        b8.config(bg=    "cyan")
        msg.showinfo("TIC TAC TOE","Congratulation!,O won the game")
        winner="O"
        check_score()
        deactivate()
        restart()

    elif b3["text"]=="O" and b6["text"]=="O" and b9["text"]=="O":
        b3.config(bg=    "cyan")
        b6.config(bg=    "cyan")
        b9.config(bg=    "cyan")
        msg.showinfo("TIC TAC TOE","Congratulation!,O won the game")
        winner="O"
        check_score()
        deactivate()
        restart()

    elif b1["text"]=="O" and b5["text"]=="O" and b9["text"]=="O":
        b1.config(bg=    "cyan")
        b5.config(bg=    "cyan")
        b9.config(bg=    "cyan")
        msg.showinfo("TIC TAC TOE","Congratulation!,O won the game")
        winner="O"
        check_score()
        deactivate()
        restart()

    elif b3["text"]=="O" and b5["text"]=="O" and b7["text"]=="O":
        b3.config(bg=    "cyan")
        b5.config(bg=    "cyan")
        b7.config(bg=    "cyan")
        msg.showinfo("TIC TAC TOE","Congratulation!,O won the game")
        winner="O"   
        check_score()
        deactivate()
        restart()

        
def check_if_tie():
    global count,b1,b2,b3,b4,b5,b6,b7,b8,b9
    if count==9 and winner!="X " or count==9 and winner!="O":
        msg.showinfo("TIC TAC TOE","IT'S A TIE")
        restart()

pointx=IntVar()
pointo=IntVar()
pointx.set(0)
pointo.set(0)
 


def check_score():
    global scorex,scoreo
    n=int(pointx.get())
    m=int(pointo.get())
    if winner=="X":
        value=(n+1)
        pointx.set(value)
    elif winner=="O":
        value=(m+1)
        pointo.set(value)
        
lblx=Label(root,text="Player X",bg="light blue",border=3).grid(row=0,column=0,columnspan=2)
scorex=Entry(root,textvariable=pointx,bg="light blue",relief=RAISED).grid(row=1,column=0,columnspan=2)
lblo=Label(root,text="Player O",bg="light blue").grid(row=0,column=1,columnspan=2)
scoreo=Entry(root,textvariable=pointo,bg="light blue",relief=RAISED).grid(row=1,column=1,columnspan=2)

count=0
click=True
def clicked(b):
    global count,click
    if b["text"]==" " and click==True:
        b["text"]="X"
        b.config(fg="red")
        click=False
        count+=1
        check_if_winner()
        check_if_tie()
        # check_score()
    elif b["text"]==" " and click==False:
        b["text"]="O"
        b.config(fg="orange")
        click=True
        count+=1
        check_if_winner()
        check_if_tie()
        # check_score()


def restart():
    global b1,b2,b3,b4,b5,b6,b7,b8,b9
    global count,click
    count=0
    click=True
    b1=Button(root,text=" ",command=lambda :clicked(b1),height=10,width=20,bg="sky blue")
    b2=Button(root,text=" ",command=lambda :clicked(b2),height=10,width=20,bg="sky blue")
    b3=Button(root,text=" ",command=lambda :clicked(b3),height=10,width=20,bg="sky blue")

    b4=Button(root,text=" ",command=lambda :clicked(b4),height=10,width=20,bg="sky blue")
    b5=Button(root,text=" ",command=lambda :clicked(b5),height=10,width=20,bg="sky blue")
    b6=Button(root,text=" ",command=lambda :clicked(b6),height=10,width=20,bg="sky blue")

    b7=Button(root,text=" ",command=lambda :clicked(b7),height=10,width=20,bg="sky blue")
    b8=Button(root,text=" ",command=lambda :clicked(b8),height=10,width=20,bg="sky blue")
    b9=Button(root,text=" ",command=lambda :clicked(b9),height=10,width=20,bg="sky blue")

    b1.config(activebackground="light blue")
    b2.config(activebackground="light blue")
    b3.config(activebackground="light blue")
    b4.config(activebackground="light blue")
    b5.config(activebackground="light blue")
    b6.config(activebackground="light blue")
    b7.config(activebackground="light blue")
    b8.config(activebackground="light blue")
    b9.config(activebackground="light blue")  

    b1.grid(row=2,column=0)
    b2.grid(row=2,column=1)
    b3.grid(row=2,column=2)
    b4.grid(row=3,column=0)
    b5.grid(row=3,column=1)
    b6.grid(row=3,column=2)
    b7.grid(row=4,column=0)
    b8.grid(row=4,column=1)
    b9.grid(row=4,column=2)

    def credit():
        msg.showinfo("CREDITS","This app is made by Srijan Kumar")

    menubar=Menu(root)
    file=Menu(menubar)
    menubar.add_cascade(label="FILE",menu=file)
    file.add_command(label="RESTART",command=restart)
    file.add_command(label="CREDIT",command=credit)
    file.add_separator()
    file.add_command(label="EXIT",command=root.destroy)
    menubar.add_command(label="NEW GAME",command=newgame)
    menubar.add_command(label="QUIT",command=quit)
   
    root.config(menu=menubar)

restart()



root.mainloop()
