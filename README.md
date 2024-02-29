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

<script>
  function sendMessage() {
    var userInput = document.getElementById('user-input').value;
    var chatMessages = document.getElementById('chat-messages');
    var userMessage = '<p>You: ' + userInput + '</p>';
    var botResponse = getBotResponse(userInput);
    var botMessage = '<p>Bot: ' + botResponse + '</p>';
    chatMessages.innerHTML += userMessage + botMessage;
    document.getElementById('user-input').value = '';
  }

  function getBotResponse(userInput) {
    // Simple chatbot logic goes here
    // For this example, I'll provide a basic hardcoded response
    if (userInput.toLowerCase().includes('hello') || userInput.toLowerCase().includes('hi')) {
      return 'Hello! How can I help you?';
    } else {
      return "I'm sorry, I didn't understand that.";
    }
  }
</script>
