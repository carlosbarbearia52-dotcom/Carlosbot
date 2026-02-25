# Carlosbot
import telebot  TOKEN = "SEU_TOKEN_AQUI" bot = telebot.TeleBot(TOKEN)  @bot.message_handler(commands=['start']) def start(message):     bot.reply_to(message, "🔥 Bot online! Seja bem-vindo.")  @bot.message_handler(func=lambda message: True) def responder(message):     bot.reply_to(message, "Você disse: " + message.text)  bot.polling()
