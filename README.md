# webbase phone scanner

### Background

In AI era, possibilities on image processing has been unleashed. To serve real-time image processing
services, projects often offer a native app / webbase app to capture user vision and process in 
backend. 

This respository aims to share a generic and effective way to implement phone scanner application. 

### Environment

This project is built base on VUE JS framework.
To run the project on local, you need to prepare nodejs and vue cli environment.

[Install vue cli](https://cli.vuejs.org/) 

### Configurations

Define your backend URL in main.vue

To maintain high availibility, you can define multiple edge backend.
The App will auto select the one with least latency as primary backend and second least latency as
secondary backend. Secondary backend will applied will primary backend timeout during runtime.

Define your upload frequency in main.vue

The App upload screen captures with upload frequency you defined. 
Caution that if upload image size * upload frequency must be **less than** available network speed.

### Customization

The app is a vuejs SPA which it serves a resultant UI of image processing in the Info component.
The scanner is paused once Info is not null, which you can immediately display result once the 
backend is successfully computed the image. Scanner is able to restart anytime by setting the
info to null again.
It is suggested to build your own UI in Info component to fit your need.

### Supported Device

This project has been tested on various devices and browser to guarantee generic support for user cases.
IPhone starts to support WebRTC in UIWebView for IOS 14.3 or above. Base on the support, we can offer
service for all devices in webbase way.

Here is the list of tested cases:

| Device    | Browser   | Special Condition |
| --------- |:---------:| -----------------:|
| Android   | Chrome    | N/A               |
| Android   | Firefox   | N/A               |
| Android   | Wechat    | N/A               |
| IOS       | Safari    | N/A               |
| IOS       | Chrome    | IOS 14.3 or above |
| IOS       | Firefox   | IOS 14.3 or above |
| IOS       | Edge      | IOS 14.3 or above |
| IOS       | Wechat    | IOS 14.3 or above |

### Example
Our team built a scanner based on this app. Here is the [live version](https://scan.i-square.co)
For information about the project, please go to [project introduction](https://www.gaccai.com)

### License
This project is licensed under the MIT License
