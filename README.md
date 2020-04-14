# CallForHelp

The *CallForHelp** application aims to help blind and low vision people to seek help in the context of work, whether in carrying out any activity or searching for information. Aid is requested through a button and the request is sent to a group of volunteers willing to help (registered in the Microsoft Teams application).

The application was developed using the Xamarin platform.

Communication between the application and Microsoft Teams is done via Logic Apps and the generation of notification to the user through Azure Functions and Azure Notification Hub.

[System Requirements for Xamarin Development](https://docs.microsoft.com/en-us/xamarin/cross-platform/get-started/requirements)

[FCM (Firebase Cloud Messaging)](https://docs.microsoft.com/en-us/xamarin/android/data-cloud/google-messaging/firebase-cloud-messaging)

[Send push notifications to Xamarin.Android apps using Notification Hubs](https://docs.microsoft.com/en-us/azure/notification-hubs/xamarin-notification-hubs-push-notifications-android-gcm#create-a-firebase-project-and-enable-firebase-cloud-messaging)

## Installation

Clone the repository, or download the project:
```
git clone https://github.com/beatrizmayumi/CallForHelp
```

## Usage
In the Constants.cs file, replace \<ENDPOINT> with the ListenConnectionString generated on your Notification Hub, and \<NOTIFICATION_HUB_NAME> with the name of your Notification Hub:

```
public const string ListenConnectionString = "<ENDPOINT>";
public const string NotificationHubName = "<NOTIFICATION_HUB_NAME>";
```

In the google-services.json file, replace the fields with “ ”, with your project data.

Example of fields to be replaced:

```
"project_info": {
"project_number": "",
"firebase_url": "",
"project_id": "",
"storage_bucket": ""
},
```

## Authors
Beatriz Matsui, Caio Melo, José Otavio Quaglio, Nei Lopez

## Licence

This project is licensed under the [MIT License](https://github.com/beatrizmayumi/CallForHelp/blob/master/LICENSE). 

--------------------------------
'\*' *The winning project of the first Accessibility Hackathon from Microsoft subsidiary in Brazil.*

