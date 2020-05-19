 
## ADD flutter for web compiled 
### replace
```html
    <img class="device-content" src="img/bk-device.jpg" alt="backgorund image"/>
```
 ### with
```html
  <iframe  class="device-content" title="Flutter compiled web app" src="web/index.html"></iframe>
```

## ADD dat pad tool into the page
```html
<iframe src="https://dartpad.dev/embed-flutter.html?id=1af7bc72cda500cee6a031339104a373&theme=dark&run=false"></iframe>
```

## ADD CHAT BOT Into a page
```html
 <!-- chat button and container -->
   <span>
    <button id="chat-button" class="chat_btn" onclick="openChatContainer()"><i class="fa fa-comments"   aria-hidden="true"></i></button>
    <div class="chat-popup" id="chat-popup">
      <div class="container chat_header">
        <a href="https://rihannake.github.io/flutter_dialogflow_bot/build/web/index.html" target="_blank">
          <i class="fas fa-2x fa-external-link-alt external-icon"></i>
        </a>
        <button class="close" onclick="closeChatContainer()"></button>
      </div>
      <div class="chat-container">
        <iframe  title="Flutter compiled web app" src="https://rihannake.github.io/flutter_dialogflow_bot/build/web/index.html">
        </iframe>
      </div>
    </div>
  </span>
```

slides

f2a4fb10b313cd822d4afb44123f6e5f
https://bit.ly/36f5miz

$ flutter create demo
$ cd demo 
$ flutter build web
$ mv web/ ../../appshowcase/

