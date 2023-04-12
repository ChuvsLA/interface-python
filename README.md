# interface-python

import customtkinter

customtkinter.set_appearance_mode('light')

janela = customtkinter.CTk()
janela.geometry('500x300')

def clique():
    print('Fazer Login')

texto = customtkinter.CTkLabel(janela, text='Login')
texto.pack(padx= 10, pady= 10)

email = customtkinter.CTkEntry(janela, placeholder_text = 'Enter your email here')
email.pack(padx= 10, pady = 10)
senha = customtkinter.CTkEntry(janela, placeholder_text = 'Enter your password here', show='*')
senha.pack(padx= 10, pady = 10)

botao = customtkinter.CTkButton(janela, fg_color="blue", text='Login')  
botao.pack(padx=10, pady=10)


janela.mainloop()

