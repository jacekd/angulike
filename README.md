angulike
========

AngularJS directives for social sharing buttons - Facebook, Google+, Twitter, Pinterest and Linked In

###Demo

To see a demo and further details go to http://jasonwatmore.com/post/2014/08/01/AngularJS-directives-for-social-sharing-buttons-Facebook-Like-GooglePlus-Twitter-and-Pinterest.aspx

###Installation

Install using bower: `bower install angulike`

Alternatively download the code and include the angulike.js file in your page.

Add the 'angulike' directive as a dependency of your AngularJS application:

```javascript
angular.module('myApp', ['angulike']);
```

###Usage

####Facebook Like

Create an empty div with the *fb-like* attribute.

```html
<div fb-like></div>
```

Optionally you can set the URL for the facebook like button to link to like this:

```html
<div fb-like="myModel.FbLikeUrl"></div>
```

###Facebook Share

Create an empty div with the *fb-share* attribute.
```html
<div fb-share></div>
```

Optional parameters:

|Parameter Name|Comment|
|--------------|-------|
|href|Valid URL to be shared|
|layout|Button layout. Please refer to [documentation](https://developers.facebook.com/docs/plugins/share-button) for all possible options|

####Google+

Create an empty div with the *google-plus* attribute.

```html
<div google-plus></div>
```

####Twitter

Create an empty div with the *tweet* attribute, the value of the attribute contains the name of the model object for the tweet text.

```html
<div tweet="myModel.Name"></div>
```

Optional parameters:

|Parameter Name|Comment|
|--------------|-------|
|text|If no scope is passed then parameter text value will be set as default text|
|url|If none set, current URL will be shared|
|count|Switch off counter with `none` as a value|
|via|optional|
|related|optional|
|hashtags|optional|

Please refer to official [documentation](https://about.twitter.com/resources/buttons#tweet) for examples.

####Pinterest

Create an empty div with the *pin-it* and *pin-it-image* attributes, the pin-it attribute contains the name of the model object for the 
description and the pin-it-image attribute contains the name of the model object for the image url:

```html
<div pin-it="myModel.Name" pin-it-image="myModel.ImageUrl"></div>
```

####Linked In

Create an empty div with the *linked-in* attribute

```html
<div linked-in></div>
```

Optional parameters:

|Parameter Name|Comment|
|--------------|-------|
|counter|position of the counter as per official [documentation](https://developer.linkedin.com/plugins/share-plugin-generator)|
|url|Valid URL to be shared|
