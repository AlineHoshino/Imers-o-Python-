Vimos sobre o yahoo finanças e a biblioteca yfinance
!pip install yfinance
import yfinance
Buscando as cotações de uma Ação
Ticker é o código de uma ação.
ticker = input('Digite o código da ação: ')
dados = yfinance.Ticker(ticker)
dados.history()
tabela = dados.history("6mo")
tabela
fechamento = tabela.Close

!pip install pyautogui 
! pip install pyperclip
import pyautogui
import pyperclip

destinatario = "seuemail@gmail.com"
assunto = "Análise diária"
mensagem = f"""
Bom dia,
Segue abaixo as análises da ação {ticker} dos últimos seis meses:
Cotação máxima: R${round(maxima,2)}
Cotação mínima: R${round(minima,2)}
Cotação atual: R${round(atual,2)}
Atenciosamente,
Seu nome.
"""

Automatizando o envio

# configurar uma pausa entre as ações do pyautogui
pyautogui.PAUSE = 3
# abrir uma nova aba
pyautogui.hotkey("ctrl", "t")
# copiar o endereço do gmail para o clipboard
pyperclip.copy("www.gmail.com")
# colar o endereço do gmail e dar um ENTER
pyautogui.hotkey("ctrl", "v")
pyautogui.press("enter")
# clicando no botão Escrever
pyautogui.click(x=, y=)
# Preenchendo o destinatário
pyperclip.copy(destinatario)
pyautogui.hotkey("ctrl", "v")
pyautogui.press("tab")
# Preenchendo o assunto
pyperclip.copy(assunto)
pyautogui.hotkey("ctrl", "v")

E-mail enviado com sucesso!
Código para descobrir as coordenados do mouse

Point(x=, y=)
pyautogui.press("tab")
# Preenchendo a mensagem
pyperclip.copy(mensagem)
pyautogui.hotkey("ctrl", "v")
# Clicar no botão Enviar
pyautogui.click(x=, y=)
# fechar a aba do gmail
pyautogui.hotkey("ctrl", "f4")
# Imprimir mensagem de enviado com sucesso
print('E-mail enviado com sucesso!')