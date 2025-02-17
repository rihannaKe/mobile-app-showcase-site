# Mobile App showcase site 
This is a website for showcasing beautifully a mobile app.

Instead of using image, gif or video, you can use the flutter compiled web app.
Checkout the [demo here and enjoy counting :)](https://rihannake.github.io/mobile-app-showcase-site/).

### How to embed a Flutter compiled intractive content?

 Clone the repo from [this repo](https://github.com/rihannaKe/mobile-app-showcase-site.git) 
 and checkout to flutter-content branch.

 After you build the web version of your Flutter app, you can deploy it anywhere you want or you can simply copy the 
 yourFlutterFolder/build/web content in the folder of this website. The main thing is that you have a reachable URL for your built flutter web app. In this demo I simply copied the flutter build web app  (the build/web folder) in this project folder. 

 At this point, instead of the images that are shown inside mobile device containers in the page, you can put the flutter compiled code simply by replacing the img tags (at line 71 and 111).

```html
  <img class="device-content" src="img/bk-device.jpg" alt="backgorund image"/>
```

  with iframe tag

```html
  <iframe  title="Flutter compiled web app" src="web/index.html"></iframe>
```

### How to embed dart.pad in your page
  To embed the dart pad dev tool in you page:
  - on your github page create a gist with your flutter code and name main.dart 
  - get the gist id 
  - use the following code to embed dart pad in you page

```html
  <iframe src="https://dartpad.dev/embed-flutter.html?id=[gist_id]"></iframe>
```
  For customizing your embedded dart pad checkout out [embedding dart pad guide](https://github.com/dart-lang/dart-pad/wiki/Embedding-Guide)

The template is built using: bootstrap 4.5.0, font-awsome 5.13.0, jquery 3.5.1,  jquery.easing 1.4.1, [html5-device-mock](https://github.com/pixelsign/html5-device-mockups) 