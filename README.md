<svg width="400" height="200" xmlns="http://www.w3.org/2000/svg">
  <foreignObject width="100%" height="100%">
    <div xmlns="http://www.w3.org/1999/xhtml">
      <h1>Hello, traveler! 👋</h1>
      <div id="chat-container">
        <div id="chat-box">
          <div id="chat-messages">
            <p>Hello! How can I assist you today?</p>
          </div>
          <input type="text" id="user-input" placeholder="Type your message...">
          <button onclick="sendMessage()">Send</button>
        </div>
      </div>
    </div>
  </foreignObject>
</svg>

<script type="text/pyscript">
  def sendMessage():
      userInput = document.getElementById('user-input').value
      chatMessages = document.getElementById('chat-messages')
      userMessage = '<p>You: ' + userInput + '</p>'
      botResponse = getBotResponse(userInput)
      botMessage = '<p>Bot: ' + botResponse + '</p>'
      chatMessages.innerHTML += userMessage + botMessage
      document.getElementById('user-input').value = ''

  def getBotResponse(userInput):
      # Simple chatbot logic goes here
      # You can use Python to generate responses and integrate it using server-side scripting
      # For this example, I'll provide a basic hardcoded response
      if 'hello' in userInput.lower() or 'hi' in userInput.lower():
          return 'Hello! How can I help you?'
      else:
          return "I'm sorry, I didn't understand that."
</script>
