# ![LOGO](logo.png) Instawell **flow**ground Connector

## Description

A generated **flow**ground connector for the Instawell API (version 1.0).

Generated from: https://api.apis.guru/v2/specs/instawell.com/1.0/swagger.json<br/>
Generated at: 2019-05-07T17:42:27+03:00

## API Description

Instawell's RESTful API gives you access to mental health professionals.

## Authorization

This API does not require authorization.

## Actions

### Create Campaign

> Create a new Campaign for an existing user or for a new user. <br/>
> <br/>
> If you are a new user and you want to create a Campaign, simply supply the email as a parameter in the body and an account will be automatically created for you. <br/>
> <br/>
> *The response will also return a an `auth_token` that you can use in subsequent requests.*<br/>
> <br/>
> If you are an existing user and you want to create a new Campaign under your existing account, then simply add the `X-instawell-token` header in the request to do this.

*Tags:* `Misc`

#### Input Parameters
* `Content-Type` - _required_

### Get Campaign

> Use this method to retrieve information about the Campaign. We return basic information like name, description and image used as well as other meta information.

*Tags:* `Misc`

#### Input Parameters
* `campaign_id` - _required_
* `Content-Type` - _required_
* `X-instawell-token` - _required_

### Get Campaign Stats

> You can use this method to  retrieve some basic stats about your Campaign. We currently return the following information<br/>
> <br/>
> - users_joined : How many uses' joined the Campaign<br/>
> - money_spent : How much money was spent on the Campaign by users.<br/>
> - plans_sold : The number of Plans that have been sold on the Campaign<br/>
> - view_count : The number of people who viewed the Campaign<br/>
> - feed : The most recent activity log of your Campaign

*Tags:* `Misc`

#### Input Parameters
* `campaign_id` - _required_
* `Content-Type` - _required_
* `X-instawell-token` - _required_

### Get Campaign Widget

> The widget code is some HTML that will allow you to embed an Instawell widget on your own website. The widget points to your Campaign and allows visitors to interact with your Campaign right from your own website. <br/>
> <br/>
> To include the widget on your website, simply copy the `embed_html` field from the response and paste it at the bottom of your website template.

*Tags:* `Misc`

#### Input Parameters
* `campaign_id` - _required_
* `Content-Type` - _required_
* `X-instawell-token` - _required_

### Update a Campaign

> The Campaign owner can update information about the Campaign. We currently allow you to update the name, description and the image used.

*Tags:* `Misc`

#### Input Parameters
* `Content-Type` - _required_
* `X-instawell-token` - _required_

### Find Plans

> Use this method to find available Plans on Instawell. Use the `category` field to filter Plans by Category. <br/>
> <br/>
> Calling this method without the `category` field will return the possible Category values. <br/>
> <br/>
> Possible category values are : mentalhealth, relationships

*Tags:* `Misc`

#### Input Parameters
* `category` - _required_
* `Content-Type` - _required_

### Request Plan

> Once you've found a Plan you like, you can make a request for it. When you make a request for it, we notify the Helper who created the Plan that there's someone waiting to chat with them. And you can start chatting with them as soon as they accept the request. <br/>
> <br/>
> The response to this method also contains a link you can use to automatically login to your account.<br/>
> <br/>
> You can call this method as a visitor or as an existing user with a valid `auth_token`. If your `auth_token` is included, we'll create the account under your existing account. Otherwise we'll create an account automatically for you and return the auth token.

*Tags:* `Misc`

#### Input Parameters
* `Content-Type` - _required_

### Get Notifications

> Use this method to retrieve your most recent notifications.

*Tags:* `Misc`

#### Input Parameters
* `Content-Type` - _required_
* `X-instawell-token` - _required_

## License

**flow**ground :- Telekom iPaaS / instawell-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
