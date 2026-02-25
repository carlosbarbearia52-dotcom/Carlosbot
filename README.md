# Carlosbot
import telebot  TOKEN = "8145367862:AAHRzQGtaYzYu1-XCokKgE5IwNb7oc1eCUQ" bot = telebot.TeleBot(TOKEN)  @bot.message_handler(commands=['start']) def start(message):     bot.reply_to(message, "🔥 Bot online! Seja bem-vindo.")  @bot.message_handler(func=lambda message: True) def responder(message):     bot.reply_to(message, "Você disse: " + message.text)  bot.polling()
