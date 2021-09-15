# webbase phone scanner

## Background

In AI era, possibilities on image processing has been unleashed. To serve real-time image processing
services, projects often offer a native app / webbase app to capture user vision and process in 
backend. 

This respository aims to share a generic and effective way to implement phone scanner application. 

## Environment

This project is built base on VUE JS framework

To run the project on local, you need to prepare nodejs and vue cli environment.
This tutorial will helps : https://cli.vuejs.org/

## Configurations

All you need to do is to define your backend URL in main.vue

To maintain high availibility, you can define multiple edge backend.
The App will auto select the one with least latency as primary backend and second least latency as
secondary backend. The 

## Recommendations

The major challenge of phone scanner application with backend is 

## Supported Device

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

