# Large Video Upload

This Python sample demonstrates the following process of uploading large video files asynchronously with the Twitter API.

1. **INIT** media upload.
2. **APPEND** chunked data.
3. **FINALIZE** media uploaded.
4. Check **STATUS** of video processing.
5. Tweet with attached video.

Large video files are longer than 30 seconds up to 140 seconds, and/or a file size larger than 15 megabytes up to 512 megabytes.

[Learn more](https://dev.twitter.com/rest/media) about the Twitter Media APIs. Pay attention to the other requirements such as encoding, frame size and video formats supported.

## Running the sample

1. Install requirements:

	```
	$ pip install -r requirements.txt
	```

2. Set the following in your ENVIRONMENT [consumer keys and access tokens](https://apps.twitter.com):

	```
	export CONSUMER_KEY='your-consumer-key'
	export CONSUMER_SECRET='your-consumer-secret'
	export ACCESS_TOKEN='your-access-token'
	export ACCESS_TOKEN_SECRET='your-access-secret'
	export ADS_ACCOUNT_ID='your-ads-url-id' (hexadecimal ID that shows in your URL on ads.twitter.com)
	export VIDEO_FILENAME='/full/local/path/to/video.mp4'
	```

3. Run script:

	```
	$ python async-upload.py
	```

4. Go to https://ads.twitter.com then select 'Creatives' and 'Media' to check for your upload.

Questions? Check our [developer discussion forums](https://https://twittercommunity.com/c/media-apis).
