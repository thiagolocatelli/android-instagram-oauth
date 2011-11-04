Android OAuth Library for Instagram Applications
---------------

![GitHub](http://thiago.grem.io/img/github/ig.png "GitHub")
![GitHub](http://thiago.grem.io/img/github/ig_oauth2.png "GitHub")
![GitHub](http://thiago.grem.io/img/github/ig_oauth3.png "GitHub")

## Usage

You can create an utility class where you can define your application credentials, like the one below:

		public class ApplicationData {
			public static final String CLIENT_ID = "";
			public static final String CLIENT_SECRET = "";
			public static final String CALLBACK_URL = "";
		}

To instantiage the main class for the oauth flow, you need to follow the code below:

		InstagramApp mApp; = new InstagramApp(this, 
			ApplicationData.CLIENT_ID, 
			ApplicationData.CLIENT_SECRET, 
			ApplicationData.CALLBACK_URL);

Once you have the main class ready for the authorization, you can start the authorization flow by calling the following method:

		mApp.authorize();

If you token is expired, you can call this method to refresh it:

		mApp.refreshToken();

To get the account list, call the following method

		mApp.getAccountList();

## Contributions

Any contribution to this project is welcome, feel free to fork and create pull requests

## Other Android Libraries

Use these libraries also to get the best for your android application

* [Android ActionBar](https://github.com/johannilsson/android-actionbar) by [Johan Nilsson](https://github.com/johannilsson)
* [Android Pull to Refresh](https://github.com/johannilsson/android-pulltorefresh) by [Johan Nilsson](https://github.com/johannilsson)
* [SwipeView](https://github.com/fry15/uk.co.jasonfry.android.tools) by [Jason Fry](https://github.com/fry15)
* [Facebook Integration](https://github.com/lorensiuswlt/AndroidFacebook) by [Lorensius](https://github.com/lorensiuswlt)
* [Twitter Integration](https://github.com/lorensiuswlt/AndroidTwitter) by [Lorensius](https://github.com/lorensiuswlt)
* [Quick Actions](https://github.com/lorensiuswlt/NewQuickAction) by [Lorensius](https://github.com/lorensiuswlt)